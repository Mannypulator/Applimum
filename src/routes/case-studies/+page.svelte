<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter } from '@lucide/svelte';

	const caseStudies = [
		{
			title: 'Orange Laundromat: Reinventing Laundry Convenience',
			desc: 'A smart laundry app that lets users schedule pickups, track orders, and receive freshly cleaned clothes within 24–48 hours all from their phone.',
			tags: ['Product Strategy', 'Mobile App', 'UX/UI Design'],
			duration: '2 months',
			link: '/case-studies/orange-laundromat'
		},
		{
			title: 'RetailCo: E-Commerce Platform Overhaul',
			desc: 'Rebuilt a legacy monolith into a modern, scalable e-commerce platform. Reduced page load times by 60% and increased conversion rate significantly.',
			tags: ['Web Development', 'UX/UI Design', 'CMS'],
			duration: '4 months',
			link: '#'
		},
		{
			title: 'SwiftMove: Logistics Tracking App',
			desc: 'Designed and built a cross-platform mobile app for real-time shipment tracking, driver management, and customer notifications.',
			tags: ['Mobile App', 'Backend', 'Product Strategy'],
			duration: '3 months',
			link: '#'
		}
	];
</script>

<svelte:head>
	<title>Case Studies – Applimum</title>
	<meta name="description" content="Explore our portfolio of successful projects." />
</svelte:head>

<!-- Navigation -->
<nav class="flex items-center justify-between px-8 py-6 max-w-7xl mx-auto">
	<a href="/" class="text-2xl font-bold tracking-tight text-brand-dark">APPLIMUM</a>
	<div class="hidden md:flex gap-8 font-medium text-slate-600">
		<a href="/" class="hover:text-brand-heading transition-colors">Home</a>
		<a href="/about" class="hover:text-brand-heading transition-colors">About Us</a>
		<a href="/service" class="hover:text-brand-heading transition-colors">Service</a>
		<a href="/case-studies" class="text-brand-heading font-semibold transition-colors">Case Studies</a>
		<a href="/contact" class="hover:text-brand-heading transition-colors">Contact</a>
	</div>
	<Button class="bg-brand-blue hover:bg-blue-800 text-white rounded-md px-6 cursor-pointer">Get Started</Button>
</nav>

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
				<div class="border border-brand-blue bg-white shadow-sm flex flex-col overflow-hidden">
					<!-- IMAGE SECTION -->
					<div class="w-full bg-[#f28e1d] flex items-center justify-center relative overflow-hidden" style="aspect-ratio: 4/3;">
						{#if i === 0}
							<!-- Note: Please save the provided image as "orange-laundromat.png" inside the "static" folder of your project -> "static/orange-laundromat.png" -->
							<img src="/orange-laudromat.svg" alt="Orange Laundromat Project Showcase" class="w-full h-full object-cover" />
						{:else}
							<div class="text-white/60 text-sm font-medium">
								[ Project Image Placeholder ]
							</div>
						{/if}
					</div>

					<!-- Content -->
					<div class="p-6 flex flex-col flex-1">
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

							<!-- CTA Button -->
							<div class="flex justify-center md:justify-start">
								<Button href={study.link} variant="outline" class="w-full md:w-auto px-6 py-2 border-brand-blue/20 text-brand-blue hover:bg-brand-blue hover:text-white transition-colors font-semibold cursor-pointer rounded-md">
									View Case Study &rarr;
								</Button>
							</div>
						</div>
					</div>
				</div>
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
					<Button class="bg-brand-blue hover:bg-blue-800 text-white px-10 py-5 text-base cursor-pointer">
						Start Your Project →
					</Button>
					<Button variant="outline" class="border-brand-blue text-brand-blue hover:bg-blue-50 px-10 py-5 text-base cursor-pointer">
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
