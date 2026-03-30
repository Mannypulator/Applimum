<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter } from '@lucide/svelte';
	import SiteHeader from '$lib/components/SiteHeader.svelte';

	const caseStudies = [
		{
			title: 'Orange Laundromat: Reinventing Laundry Convenience',
			desc: 'A smart laundry app that lets users schedule pickups, track orders, and receive freshly cleaned clothes within 24-48 hours all from their phone.',
			tags: ['Product Strategy', 'Mobile App', 'UX/UI Design'],
			duration: '2 months',
			link: '/case-studies/orange-laundromat',
			ctaLabel: 'View Case Study ->',
			visualLabel: 'Orange Laundromat',
			visualMeta: 'Pickup, tracking, delivery',
			visualTone: 'orange'
		},
		{
			title: 'RetailCo: E-Commerce Platform Overhaul',
			desc: 'Rebuilt a legacy monolith into a modern, scalable e-commerce platform. Reduced page load times by 60% and increased conversion rate significantly.',
			tags: ['Web Development', 'UX/UI Design', 'CMS'],
			duration: '4 months',
			link: '/case-studies/retailco',
			ctaLabel: 'View Case Study ->',
			visualLabel: 'RetailCo',
			visualMeta: '60% faster pages',
			visualTone: 'blue'
		},
		{
			title: 'SwiftMove: Logistics Tracking App',
			desc: 'Designed and built a cross-platform mobile app for real-time shipment tracking, driver management, and customer notifications.',
			tags: ['Mobile App', 'Backend', 'Product Strategy'],
			duration: '3 months',
			link: '/case-studies/swiftmove',
			ctaLabel: 'View Case Study ->',
			visualLabel: 'SwiftMove',
			visualMeta: 'Realtime logistics visibility',
			visualTone: 'slate'
		}
	];
</script>

<svelte:head>
	<title>Case Studies – Applimum</title>
	<meta name="description" content="Explore our portfolio of successful projects." />
</svelte:head>

<SiteHeader />

<!-- ===== HERO ===== -->
<section class="relative overflow-hidden bg-gradient-to-br from-white via-brand-light to-white pt-16 pb-20">
	<!-- Decorative dots -->
	<div class="absolute top-8 right-8 grid grid-cols-5 gap-3 opacity-30 pointer-events-none" aria-hidden="true">
		{#each { length: 25 } as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>
	<div class="absolute bottom-8 left-8 grid grid-cols-5 gap-3 opacity-30 pointer-events-none" aria-hidden="true">
		{#each { length: 25 } as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>

	<div class="max-w-5xl mx-auto px-6 text-center relative z-10">
		<h1 class="text-5xl md:text-7xl font-extrabold leading-tight tracking-tight text-brand-blue mb-6">
			Real <span class="text-brand-orange">Results,</span> Real<br />
			<span class="text-brand-orange">Impact.</span>
		</h1>
		<p class="text-slate-500 text-lg max-w-3xl mx-auto">
			Explore our portfolio of successful projects where innovation meets execution. Each case study represents our commitment to delivering exceptional digital solutions.
		</p>
	</div>
</section>

<!-- ===== CASE STUDY CARDS ===== -->
<section class="py-20 bg-white">
	<div class="max-w-7xl mx-auto px-6">
		<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
			{#each caseStudies as study, i}
				<a
					href={study.link}
					aria-label={`View case study for ${study.title}`}
					class="group flex flex-col overflow-hidden rounded-[2rem] border border-brand-blue/15 bg-linear-to-b from-white to-slate-50/70 shadow-[0_18px_55px_-28px_rgba(0,68,147,0.42)] transition-all duration-200 hover:-translate-y-1 hover:border-brand-blue/30 hover:shadow-[0_28px_80px_-34px_rgba(0,68,147,0.52)] focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-brand-blue/40"
				>
					<!-- IMAGE SECTION -->
					<div
						class={`relative flex w-full items-center justify-center overflow-hidden ${
							study.visualTone === 'orange'
								? 'bg-[#f28e1d]'
								: study.visualTone === 'blue'
									? 'bg-linear-to-br from-[#0f4c81] via-[#155fa0] to-[#4ea8de]'
									: 'bg-linear-to-br from-slate-800 via-slate-700 to-slate-500'
						}`}
						style="aspect-ratio: 4/3;"
					>
						{#if i === 0}
							<img src="/orange-laudromat.svg" alt="Orange Laundromat Project Showcase" class="w-full h-full object-cover" />
						{:else}
							<div class="absolute inset-0 opacity-20">
								<div class="absolute left-6 top-6 h-14 w-14 rounded-full border border-white/30"></div>
								<div class="absolute right-8 top-10 h-24 w-24 rounded-3xl border border-white/20"></div>
								<div class="absolute bottom-6 left-10 h-20 w-20 rounded-2xl border border-white/20"></div>
							</div>
							<div class="relative z-10 px-6 text-center text-white">
								<p class="text-sm font-semibold uppercase tracking-[0.3em] text-white/70">
									Case Study
								</p>
								<h2 class="mt-3 text-3xl font-extrabold tracking-tight">
									{study.visualLabel}
								</h2>
								<p class="mt-3 text-sm font-medium text-white/80">{study.visualMeta}</p>
							</div>
						{/if}
					</div>

					<!-- Content -->
					<div class="flex flex-1 flex-col p-7">
						<!-- Title & Logo -->
						<div class="flex items-start gap-3 mb-4">
							{#if i === 0}
							<div class="w-7 h-7 rounded-full bg-brand-orange/10 flex items-center justify-center text-brand-orange shrink-0 mt-0.5">
								<svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"></circle><path d="m12 2 4 10H8z"></path><path d="M12 22V12"></path></svg>
							</div>
							{:else}
							<div class="w-7 h-7 rounded-full bg-brand-blue/10 flex items-center justify-center text-brand-blue shrink-0 mt-0.5">
								<svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path><polyline points="3.27 6.96 12 12.01 20.73 6.96"></polyline><line x1="12" x2="12" y1="22.08" y2="12"></line></svg>
							</div>
							{/if}
							<h2 class="text-[17px] font-bold text-slate-800 leading-snug">{study.title}</h2>
						</div>

						<!-- Description -->
						<p class="text-slate-500 text-[14px] leading-relaxed mb-6 flex-1">
							{study.desc}
						</p>

						<!-- Tags -->
						<div class="flex flex-wrap gap-2 mb-6">
							{#each study.tags as tag}
								<span class="text-[12px] font-medium px-2.5 py-1 rounded bg-[#E0F2FE] text-[#0369A1]">
									{tag}
								</span>
							{/each}
						</div>

						<!-- Duration & Footer -->
						<div class="mt-auto">
							<hr class="border-slate-100 mb-4" />
							<div class="text-[13px] text-slate-500 mb-6">
								Duration: <span class="font-medium text-slate-700">{study.duration}</span>
							</div>

							<div class="flex justify-center md:justify-start">
								<span class="inline-flex w-full items-center justify-center rounded-full border border-brand-blue/20 px-6 py-2.5 font-semibold text-brand-blue transition-colors group-hover:bg-brand-blue group-hover:text-white md:w-auto">
									{study.ctaLabel}
								</span>
							</div>
						</div>
					</div>
				</a>
			{/each}
		</div>
	</div>
</section>

<!-- ===== CTA ===== -->
<section class="py-16 bg-white">
	<div class="max-w-5xl mx-auto px-6">
		<div class="relative rounded-2xl border border-slate-200 bg-white shadow-sm px-12 py-16 text-center overflow-hidden">
			<!-- Decorative dot corners -->
			<div class="absolute top-4 left-4 grid grid-cols-6 gap-2.5 opacity-20 pointer-events-none" aria-hidden="true">
				{#each { length: 36 } as _}
					<span class="w-1 h-1 rounded-full bg-slate-400 inline-block"></span>
				{/each}
			</div>
			<div class="absolute bottom-4 right-4 grid grid-cols-6 gap-2.5 opacity-20 pointer-events-none" aria-hidden="true">
				{#each { length: 36 } as _}
					<span class="w-1 h-1 rounded-full bg-slate-400 inline-block"></span>
				{/each}
			</div>

			<div class="relative z-10">
				<h2 class="text-3xl md:text-4xl font-extrabold text-brand-heading mb-4">
					Ready to Be Our Next Success Story?
				</h2>
				<p class="text-slate-500 mb-10 max-w-lg mx-auto">
					Let's turn your vision into a product that delivers real, measurable results for your business.
				</p>
				<div class="flex flex-col sm:flex-row justify-center gap-4">
					<Button
						href="/contact"
						class="bg-brand-blue hover:bg-blue-800 text-white px-10 py-5 text-base cursor-pointer"
					>
						Start Your Project →
					</Button>
					<Button
						href="/contact"
						variant="outline"
						class="border-brand-blue text-brand-blue hover:bg-blue-50 px-10 py-5 text-base cursor-pointer"
					>
						Contact Us
					</Button>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- ===== FOOTER ===== -->
<footer class="bg-brand-dark text-slate-300 py-16 text-sm">
	<div class="container mx-auto px-8 grid grid-cols-1 md:grid-cols-4 gap-10">
		<div class="space-y-4 md:col-span-1">
			<h3 class="text-xl font-bold text-white tracking-tight">APPLIMUM</h3>
			<p class="text-slate-400 text-sm leading-relaxed">
				Software Engineering and Consulting.<br />
				Building reliable digital solutions.
			</p>
		</div>

		<div>
			<h4 class="font-semibold text-white mb-5 text-sm">Quick Links</h4>
			<ul class="space-y-3">
				<li><a href="/about" class="hover:text-white transition-colors">About Us</a></li>
				<li><a href="/service" class="hover:text-white transition-colors">Service</a></li>
				<li><a href="/case-studies" class="text-brand-blue hover:text-brand-blue/80 transition-colors">Case Studies</a></li>
			</ul>
		</div>

		<div>
			<h4 class="font-semibold text-white mb-5 text-sm">Contact</h4>
			<ul class="space-y-3">
				<li class="flex items-center gap-2">
					<Mail class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="mailto:info@applimum.com" class="hover:text-brand-blue transition-colors">info@applimum.com</a>
				</li>
				<li class="flex items-center gap-2">
					<Phone class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="tel:+23409039413344" class="hover:text-brand-blue transition-colors">+234-09039413344</a>
				</li>
				<li class="flex items-center gap-2">
					<Phone class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="tel:+2348076875450" class="hover:text-brand-blue transition-colors">08076875450</a>
				</li>
			</ul>
		</div>

		<div>
			<h4 class="font-semibold text-white mb-5 text-sm">Services</h4>
			<ul class="space-y-3">
				<li class="flex items-center gap-2">
					<Linkedin class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="https://linkedin.com" target="_blank" rel="noreferrer" class="hover:text-brand-blue transition-colors">LinkedIn</a>
				</li>
				<li class="flex items-center gap-2">
					<Instagram class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="https://instagram.com" target="_blank" rel="noreferrer" class="hover:text-brand-blue transition-colors">Instagram</a>
				</li>
				<li class="flex items-center gap-2">
					<Twitter class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="https://twitter.com" target="_blank" rel="noreferrer" class="hover:text-brand-blue transition-colors">X (formerly Twitter)</a>
				</li>
			</ul>
		</div>
	</div>

	<div class="container mx-auto px-8 mt-12 pt-6 border-t border-slate-800/50 flex flex-col md:flex-row justify-between items-center text-xs text-slate-500">
		<p>© <strong class="text-slate-300">Applimum {new Date().getFullYear()}.</strong> All rights reserved.</p>
		<a href="/privacy" class="hover:text-brand-blue transition-colors mt-2 md:mt-0">Privacy Policy</a>
	</div>
</footer>
