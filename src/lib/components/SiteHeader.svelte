<script lang="ts">
	import { page } from '$app/state';
	import { Menu, X } from '@lucide/svelte';
	import { Button } from '$lib/components/ui/button';

	type NavItem = {
		href: string;
		label: string;
		match?: 'exact' | 'prefix';
	};

	const navItems: NavItem[] = [
		{ href: '/', label: 'Home' },
		{ href: '/about', label: 'About Us' },
		{ href: '/service', label: 'Service' },
		{ href: '/case-studies', label: 'Case Studies', match: 'prefix' },
		{ href: '/contact', label: 'Contact' }
	];

	let menuOpen = $state(false);

	function isActive({ href, match = 'exact' }: NavItem) {
		const pathname = page.url.pathname;

		if (match === 'prefix') {
			return pathname === href || pathname.startsWith(`${href}/`);
		}

		return pathname === href;
	}

	function toggleMenu() {
		menuOpen = !menuOpen;
	}

	function closeMenu() {
		menuOpen = false;
	}
</script>

<nav class="relative mx-auto max-w-7xl px-4 py-6 sm:px-6 lg:px-8">
	<div class="flex items-center justify-between gap-4">
		<a href="/" class="text-2xl font-bold tracking-tight text-brand-dark">APPLIMUM</a>

		<div class="hidden items-center gap-8 font-medium text-slate-600 md:flex">
			{#each navItems as item}
				<a
					href={item.href}
					class={`transition-colors ${
						isActive(item)
							? 'font-semibold text-brand-heading'
							: 'hover:text-brand-heading'
					}`}
				>
					{item.label}
				</a>
			{/each}
		</div>

		<div class="hidden md:block">
			<Button
				href="/contact"
				class="cursor-pointer rounded-md bg-brand-blue px-6 text-white hover:bg-blue-800"
			>
				Get Started
			</Button>
		</div>

		<Button
			variant="ghost"
			size="icon"
			class="border border-brand-blue/15 text-brand-blue shadow-none hover:bg-brand-light md:hidden"
			aria-controls="mobile-navigation"
			aria-expanded={menuOpen}
			aria-label={menuOpen ? 'Close navigation menu' : 'Open navigation menu'}
			onclick={toggleMenu}
		>
			{#if menuOpen}
				<X class="size-5" />
			{:else}
				<Menu class="size-5" />
			{/if}
		</Button>
	</div>

	{#if menuOpen}
		<div
			id="mobile-navigation"
			class="mt-4 rounded-[1.75rem] border border-brand-blue/10 bg-white/95 p-4 shadow-xl shadow-brand-blue/10 ring-1 ring-brand-blue/5 backdrop-blur md:hidden"
		>
			<div class="flex flex-col gap-2">
				{#each navItems as item}
					<a
						href={item.href}
						class={`rounded-2xl px-4 py-3 text-sm font-semibold transition-colors ${
							isActive(item)
								? 'bg-brand-blue text-white'
								: 'bg-slate-50 text-slate-700 hover:bg-brand-light hover:text-brand-heading'
						}`}
						onclick={closeMenu}
					>
						{item.label}
					</a>
				{/each}
			</div>

			<Button
				href="/contact"
				class="mt-4 w-full cursor-pointer rounded-2xl bg-brand-blue py-3 text-white hover:bg-blue-800"
				onclick={closeMenu}
			>
				Get Started
			</Button>
		</div>
	{/if}
</nav>
