<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter, ArrowLeft } from '@lucide/svelte';
	import SiteHeader from '$lib/components/SiteHeader.svelte';
</script>

<svelte:head>
	<title>RetailCo Case Study - Applimum</title>
	<meta
		name="description"
		content="See how Applimum helped RetailCo modernize its e-commerce platform and improve performance."
	/>
</svelte:head>

<SiteHeader />

<main class="max-w-6xl mx-auto px-6 pb-24">
	<div class="mb-8 mt-4">
		<a
			href="/case-studies"
			class="inline-flex flex-row items-center gap-2 rounded-md border border-brand-blue/30 px-4 py-2 text-sm font-semibold text-brand-blue transition-colors hover:bg-brand-blue/5"
		>
			<ArrowLeft class="w-4 h-4" />
			Back
		</a>
	</div>

	<div class="relative mb-20 overflow-hidden rounded-[2rem] bg-linear-to-br from-[#0f4c81] via-[#145d9d] to-[#4ea8de] p-10 text-white md:p-16">
		<div class="grid gap-10 md:grid-cols-2 md:items-center">
			<div class="z-10 flex flex-col items-start gap-6">
				<div class="rounded-full border border-white/20 bg-white/10 px-4 py-2 text-sm font-semibold uppercase tracking-[0.25em]">
					Commerce Transformation
				</div>
				<h1 class="text-4xl font-extrabold leading-tight md:text-5xl">
					RetailCo: E-Commerce Platform Overhaul
				</h1>
				<p class="max-w-xl text-lg leading-relaxed text-white/85">
					We helped RetailCo replace a slow, fragile storefront with a faster commerce
					experience designed for merchandising speed, operational clarity, and sustained
					conversion growth.
				</p>
			</div>

			<div class="grid gap-4 rounded-[1.75rem] border border-white/15 bg-white/8 p-6 backdrop-blur-sm">
				<div class="grid grid-cols-2 gap-4">
					<div class="rounded-2xl bg-white/12 p-5">
						<p class="text-xs font-semibold uppercase tracking-[0.25em] text-white/65">
							Page Speed
						</p>
						<p class="mt-3 text-3xl font-extrabold">60%</p>
						<p class="mt-2 text-sm text-white/75">Faster page load times after launch</p>
					</div>
					<div class="rounded-2xl bg-white/12 p-5">
						<p class="text-xs font-semibold uppercase tracking-[0.25em] text-white/65">
							Release Flow
						</p>
						<p class="mt-3 text-3xl font-extrabold">1</p>
						<p class="mt-2 text-sm text-white/75">Unified stack for storefront and content</p>
					</div>
				</div>
				<div class="rounded-[1.5rem] border border-white/15 bg-slate-950/20 p-5">
					<p class="text-sm font-semibold uppercase tracking-[0.2em] text-white/60">
						What changed
					</p>
					<ul class="mt-4 space-y-3 text-sm text-white/80">
						<li>Composable storefront architecture</li>
						<li>Improved mobile browsing and checkout flow</li>
						<li>Better merchandising and campaign publishing</li>
					</ul>
				</div>
			</div>
		</div>
	</div>

	<div class="mb-20 grid gap-12 md:grid-cols-2 md:items-start">
		<div class="rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">Client Overview</h2>
			<p class="text-lg leading-relaxed text-slate-600">
				RetailCo is a growing retailer with a broad product catalog, recurring promotional
				campaigns, and a business model that depends on fast seasonal updates. Their existing
				platform had become difficult to maintain, expensive to scale, and too slow for the
				customer experience they wanted to deliver.
			</p>
		</div>
		<div class="rounded-2xl border border-slate-200 bg-slate-50 p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">The Challenge</h2>
			<ul class="list-disc space-y-3 pl-5 leading-relaxed text-slate-600">
				<li>Legacy storefront pages loaded too slowly, especially on mobile.</li>
				<li>Campaign launches required too much engineering support.</li>
				<li>Search, category browsing, and checkout lacked consistency.</li>
				<li>Teams needed better visibility into content and product updates.</li>
			</ul>
		</div>
	</div>

	<div class="mb-20 grid gap-12 md:grid-cols-2 md:items-start">
		<div class="rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">Our Approach</h2>
			<div class="space-y-6 text-slate-600">
				<div>
					<p class="font-semibold text-slate-800">1. Audit and prioritization</p>
					<p class="mt-2 leading-relaxed">
						We mapped the highest-friction journeys across landing pages, category views,
						product pages, and checkout to focus on the biggest performance and usability wins.
					</p>
				</div>
				<div>
					<p class="font-semibold text-slate-800">2. Experience redesign</p>
					<p class="mt-2 leading-relaxed">
						We simplified page structure, improved visual hierarchy, and tightened the mobile
						buying journey so customers could move from discovery to checkout with less friction.
					</p>
				</div>
				<div>
					<p class="font-semibold text-slate-800">3. Scalable implementation</p>
					<p class="mt-2 leading-relaxed">
						We shaped the platform around reusable merchandising blocks and cleaner release
						workflows so new campaigns could go live faster without one-off engineering work.
					</p>
				</div>
			</div>
		</div>
		<div class="rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">The Solution</h2>
			<ul class="space-y-4 text-slate-600">
				<li><strong class="text-slate-800">Faster storefront rendering:</strong> leaner page composition and improved asset delivery.</li>
				<li><strong class="text-slate-800">Better product discovery:</strong> cleaner category navigation, filtering, and search behavior.</li>
				<li><strong class="text-slate-800">Stronger merchandising tools:</strong> reusable content sections for launches and promotions.</li>
				<li><strong class="text-slate-800">More confident releases:</strong> fewer breakpoints between design, content, and engineering teams.</li>
			</ul>
		</div>
	</div>

	<div class="mb-20 rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
		<h2 class="mb-6 text-2xl font-bold text-brand-heading">The Impact</h2>
		<div class="grid gap-4 md:grid-cols-2">
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">60%</p>
				<p class="mt-2 text-slate-600">Reduction in page load time on key storefront journeys.</p>
			</div>
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Higher</p>
				<p class="mt-2 text-slate-600">Conversion confidence through cleaner browsing and checkout flows.</p>
			</div>
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Faster</p>
				<p class="mt-2 text-slate-600">Campaign publishing for merchandising and marketing teams.</p>
			</div>
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Stronger</p>
				<p class="mt-2 text-slate-600">Platform foundations for future commerce growth.</p>
			</div>
		</div>
	</div>

	<div class="relative overflow-hidden rounded-[2rem] bg-brand-light p-12 text-center">
		<h2 class="relative z-10 mb-6 text-4xl font-extrabold text-brand-dark md:text-5xl">
			Need a stronger digital storefront?
		</h2>
		<p class="relative z-10 mx-auto mb-10 max-w-3xl text-lg leading-relaxed text-slate-600">
			If your commerce experience is slowing down growth, we can help you redesign the
			customer journey and modernize the platform behind it.
		</p>
		<Button
			href="/contact"
			class="relative z-10 cursor-pointer rounded-md bg-brand-blue px-8 py-6 text-lg font-semibold text-white shadow-lg shadow-brand-blue/20 hover:bg-blue-800"
		>
			Start Building Today ->
		</Button>
	</div>
</main>

<footer class="bg-brand-dark py-16 text-sm text-slate-300">
	<div class="container mx-auto grid w-full max-w-7xl grid-cols-1 gap-10 px-8 md:grid-cols-4">
		<div class="space-y-4 md:col-span-1">
			<h3 class="text-xl font-bold tracking-tight text-white">APPLIMUM</h3>
			<p class="text-sm leading-relaxed text-slate-400">
				Software Engineering and Consulting.<br />
				Building reliable digital solutions.
			</p>
		</div>

		<div>
			<h4 class="mb-5 text-sm font-semibold text-white">Quick Links</h4>
			<ul class="space-y-3">
				<li><a href="/about" class="transition-colors hover:text-white">About Us</a></li>
				<li><a href="/service" class="transition-colors hover:text-white">Service</a></li>
				<li><a href="/case-studies" class="transition-colors hover:text-white">Case Studies</a></li>
			</ul>
		</div>

		<div>
			<h4 class="mb-5 text-sm font-semibold text-white">Contact</h4>
			<ul class="space-y-3">
				<li class="flex items-center gap-2">
					<Mail class="w-4 h-4 shrink-0 text-slate-500" />
					<a href="mailto:info@applimum.com" class="transition-colors hover:text-brand-blue">info@applimum.com</a>
				</li>
				<li class="flex items-center gap-2">
					<Phone class="w-4 h-4 shrink-0 text-slate-500" />
					<a href="tel:+23409039413344" class="transition-colors hover:text-brand-blue">+234-09039413344</a>
				</li>
				<li class="flex items-center gap-2">
					<Phone class="w-4 h-4 shrink-0 text-slate-500" />
					<a href="tel:+2348076875450" class="transition-colors hover:text-brand-blue">08076875450</a>
				</li>
			</ul>
		</div>

		<div>
			<h4 class="mb-5 text-sm font-semibold text-white">Services</h4>
			<ul class="space-y-3">
				<li class="flex items-center gap-2">
					<Linkedin class="w-4 h-4 shrink-0 text-slate-500" />
					<a href="https://linkedin.com" target="_blank" rel="noreferrer" class="transition-colors hover:text-brand-blue">LinkedIn</a>
				</li>
				<li class="flex items-center gap-2">
					<Instagram class="w-4 h-4 shrink-0 text-slate-500" />
					<a href="https://instagram.com" target="_blank" rel="noreferrer" class="transition-colors hover:text-brand-blue">Instagram</a>
				</li>
				<li class="flex items-center gap-2">
					<Twitter class="w-4 h-4 shrink-0 text-slate-500" />
					<a href="https://twitter.com" target="_blank" rel="noreferrer" class="transition-colors hover:text-brand-blue">X (formerly Twitter)</a>
				</li>
			</ul>
		</div>
	</div>

	<div class="container mx-auto mt-12 flex max-w-7xl flex-col items-center justify-between border-t border-slate-800/50 px-8 pt-6 text-xs text-slate-500 md:flex-row">
		<p>
			© <strong class="text-slate-300">Applimum {new Date().getFullYear()}.</strong> All rights reserved.
		</p>
		<a href="/privacy" class="mt-2 transition-colors hover:text-brand-blue md:mt-0">Privacy Policy</a>
	</div>
</footer>
