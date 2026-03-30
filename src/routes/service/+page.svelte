<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter } from '@lucide/svelte';

	// Service Icons
	import ProjectMgmtIcon from '$lib/components/icons/ProjectMgmtIcon.svelte';
	import WebDevIcon from '$lib/components/icons/WebDevIcon.svelte';
	import MobileAppIcon from '$lib/components/icons/MobileAppIcon.svelte';
	import UiUxIcon from '$lib/components/icons/UiUxIcon.svelte';

	const topServices = [
		{
			icon: ProjectMgmtIcon,
			title: 'Project Management Consulting',
			desc: 'Need strategic advice on your next tech move? We provide clear guidance on roadmaps, resources, and risk. We help you establish predictable timelines and deliver success from day one.'
		},
		{
			icon: WebDevIcon,
			title: 'Web Development: Your Digital Foundation for Growth',
			desc: 'We build custom websites and web applications that are robust, scalable, and tailored to your specific business needs.'
		},
		{
			icon: MobileAppIcon,
			title: 'Mobile Application Development: Building Apps That Stand Out',
			desc: "A great app is more than just code, it's a solution that solves a real problem. We build high-performance mobile applications for both iOS and Android, focusing on speed, security, and a flawless user experience."
		}
	];
</script>

<svelte:head>
	<title>Service – Applimum</title>
	<meta
		name="description"
		content="Explore Applimum's services — from a spark of an idea to fully-built digital solutions."
	/>
</svelte:head>

<!-- Navigation -->
<nav class="flex items-center justify-between px-8 py-6 max-w-7xl mx-auto">
	<a href="/" class="text-2xl font-bold tracking-tight text-brand-dark">APPLIMUM</a>
	<div class="hidden md:flex gap-8 font-medium text-slate-600">
		<a href="/" class="hover:text-brand-heading transition-colors">Home</a>
		<a href="/about" class="hover:text-brand-heading transition-colors">About Us</a>
		<a href="/service" class="text-brand-heading font-semibold transition-colors">Service</a>
		<a href="/case-studies" class="hover:text-brand-heading transition-colors">Case Studies</a>
		<a href="/contact" class="hover:text-brand-heading transition-colors">Contact</a>
	</div>
	<Button class="bg-brand-blue hover:bg-blue-800 text-white rounded-md px-6 cursor-pointer">
		Get Started
	</Button>
</nav>

<!-- ===== HERO ===== -->
<section class="relative overflow-hidden bg-gradient-to-br from-white via-brand-light to-white pt-16 pb-12">
	<!-- Decorative dots top-right -->
	<div
		class="absolute top-8 right-8 grid grid-cols-5 gap-3 opacity-30 pointer-events-none"
		aria-hidden="true"
	>
		{#each { length: 25 } as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>
	<!-- Decorative dots bottom-left -->
	<div
		class="absolute bottom-8 left-8 grid grid-cols-5 gap-3 opacity-30 pointer-events-none"
		aria-hidden="true"
	>
		{#each { length: 25 } as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>

	<div class="max-w-5xl mx-auto px-6 relative z-10">
		<h1
			class="text-5xl md:text-7xl font-extrabold leading-tight tracking-tight text-brand-heading mb-8"
		>
			From a Spark of an <span class="text-brand-orange">Idea</span><br />
			to a <span class="text-brand-orange">Fully-Built Solution.</span>
		</h1>
		<p class="text-slate-500 text-lg max-w-xl">
			We offer a range of services to help you succeed in the digital landscape.
		</p>
	</div>
</section>

<!-- ===== SERVICE CARDS ===== -->
<section class="py-16 bg-white">
	<div class="max-w-5xl mx-auto px-6 flex flex-col gap-6">
		<!-- Top 3 cards -->
		<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
			{#each topServices as service}
				<div
					class="rounded-2xl border border-slate-200 bg-white shadow-sm p-6 hover:shadow-md transition-shadow"
				>
					<div class="mb-4">
						<service.icon class="w-12 h-12" />
					</div>
					<h3 class="font-bold text-brand-heading text-base leading-snug mb-3">{service.title}</h3>
					<p class="text-slate-500 text-sm leading-relaxed">{service.desc}</p>
				</div>
			{/each}
		</div>

		<!-- Full-width UI/UX card -->
		<div
			class="rounded-2xl border border-slate-200 bg-white shadow-sm p-6 hover:shadow-md transition-shadow"
		>
			<div class="flex items-start gap-4">
				<div class="shrink-0">
					<UiUxIcon class="w-12 h-12" />
				</div>
				<div>
					<h3 class="font-bold text-brand-heading text-base mb-2">
						UI/UX Design: Creating Experiences People Love.
					</h3>
					<p class="text-slate-500 text-sm leading-relaxed max-w-3xl">
						Your software's success depends on its user experience. We don't just design interfaces,
						we create intuitive, engaging experiences that make your customers' lives easier and keep
						them coming back. Our user-centered design approach ensures your digital product is not
						only beautiful but also effective and driving conversion, and building brand loyalty.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>

<!-- ===== JOIN OUR MISSION CTA ===== -->
<section class="py-16 bg-white">
	<div class="max-w-5xl mx-auto px-6">
		<div
			class="relative rounded-2xl border border-slate-200 bg-white shadow-sm px-12 py-16 text-center overflow-hidden"
		>
			<!-- Decorative dot grid corners inside card -->
			<div
				class="absolute top-4 left-4 grid grid-cols-6 gap-2.5 opacity-20 pointer-events-none"
				aria-hidden="true"
			>
				{#each { length: 36 } as _}
					<span class="w-1 h-1 rounded-full bg-slate-400 inline-block"></span>
				{/each}
			</div>
			<div
				class="absolute bottom-4 right-4 grid grid-cols-6 gap-2.5 opacity-20 pointer-events-none"
				aria-hidden="true"
			>
				{#each { length: 36 } as _}
					<span class="w-1 h-1 rounded-full bg-slate-400 inline-block"></span>
				{/each}
			</div>

			<div class="relative z-10">
				<h2 class="text-3xl md:text-4xl font-extrabold text-brand-heading mb-4">
					Join Our Mission
				</h2>
				<p class="text-slate-500 mb-10 max-w-lg mx-auto">
					Ready to build the future of digital experiences? Let's turn your vision into a scalable
					product that drives real results.
				</p>
				<Button
					class="bg-brand-blue hover:bg-blue-800 text-white px-10 py-5 text-base cursor-pointer"
				>
					Start Building Today →
				</Button>
			</div>
		</div>
	</div>
</section>

<!-- ===== FOOTER ===== -->
<footer class="bg-brand-dark text-slate-300 py-16 text-sm">
	<div class="container mx-auto px-8 grid grid-cols-1 md:grid-cols-4 gap-10">
		<!-- Brand -->
		<div class="space-y-4 md:col-span-1">
			<h3 class="text-xl font-bold text-white tracking-tight">APPLIMUM</h3>
			<p class="text-slate-400 text-sm leading-relaxed">
				Software Engineering and Consulting.<br />
				Building reliable digital solutions.
			</p>
		</div>

		<!-- Quick Links -->
		<div>
			<h4 class="font-semibold text-white mb-5 text-sm">Quick Links</h4>
			<ul class="space-y-3">
				<li><a href="/about" class="hover:text-white transition-colors">About Us</a></li>
				<li><a href="/service" class="hover:text-white transition-colors">Service</a></li>
				<li><a href="/#case-studies" class="hover:text-white transition-colors">Case Studies</a></li>
			</ul>
		</div>

		<!-- Contact -->
		<div>
			<h4 class="font-semibold text-white mb-5 text-sm">Contact</h4>
			<ul class="space-y-3">
				<li class="flex items-center gap-2">
					<Mail class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="mailto:info@applimum.com" class="hover:text-brand-blue transition-colors">
						info@applimum.com
					</a>
				</li>
				<li class="flex items-center gap-2">
					<Phone class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="tel:+23409039413344" class="hover:text-brand-blue transition-colors">
						+234-09039413344
					</a>
				</li>
				<li class="flex items-center gap-2">
					<Phone class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="tel:+2348076875450" class="hover:text-brand-blue transition-colors">
						08076875450
					</a>
				</li>
			</ul>
		</div>

		<!-- Services / Socials -->
		<div>
			<h4 class="font-semibold text-white mb-5 text-sm">Services</h4>
			<ul class="space-y-3">
				<li class="flex items-center gap-2">
					<Linkedin class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="https://linkedin.com" class="hover:text-brand-blue transition-colors" target="_blank" rel="noreferrer">LinkedIn</a>
				</li>
				<li class="flex items-center gap-2">
					<Instagram class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="https://instagram.com" class="hover:text-brand-blue transition-colors" target="_blank" rel="noreferrer">Instagram</a>
				</li>
				<li class="flex items-center gap-2">
					<Twitter class="w-4 h-4 text-slate-500 shrink-0" />
					<a href="https://twitter.com" class="hover:text-brand-blue transition-colors" target="_blank" rel="noreferrer">X (formerly Twitter)</a>
				</li>
			</ul>
		</div>
	</div>

	<!-- Bottom bar -->
	<div
		class="container mx-auto px-8 mt-12 pt-6 border-t border-slate-800/50 flex flex-col md:flex-row justify-between items-center text-xs text-slate-500"
	>
		<p>
			© <strong class="text-slate-300">Applimum {new Date().getFullYear()}.</strong> All rights reserved.
		</p>
		<a href="/privacy" class="hover:text-brand-blue transition-colors mt-2 md:mt-0">Privacy Policy</a>
	</div>
</footer>
