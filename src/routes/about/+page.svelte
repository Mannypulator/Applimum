<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Badge } from '$lib/components/ui/badge';
	import { Mail, Phone, Linkedin, Instagram, Twitter } from '@lucide/svelte';

	// About Us Icons
	import PartnershipIcon from '$lib/components/icons/PartnershipIcon.svelte';
	import IntegrityIcon from '$lib/components/icons/IntegrityIcon.svelte';
	import CraftsmanshipIcon from '$lib/components/icons/CraftsmanshipIcon.svelte';
	import EmpathyIcon from '$lib/components/icons/EmpathyIcon.svelte';
	import ProgressIcon from '$lib/components/icons/ProgressIcon.svelte';
	import AgileIcon from '$lib/components/icons/AgileIcon.svelte';

	const principles = [
		{
			icon: PartnershipIcon,
			title: 'Partnership',
			desc: "We don't just work for you; we work with you. We're an extension of your team, and your goals become our goals."
		},
		{
			icon: IntegrityIcon,
			title: 'Integrity',
			desc: "We're honest and transparent. We'll always give you our straightforward advice, even if it's not what you expected."
		},
		{
			icon: CraftsmanshipIcon,
			title: 'Craftsmanship & Resilience',
			desc: "We're passionate about what we build. We pay attention to the details, ensuring every line of code is clean, robust and built to last."
		},
		{
			icon: EmpathyIcon,
			title: 'Empathy & User-Centricity',
			desc: "We believe great software is built on understanding. Before we write a single line of code, we take the time to truly understand your customers' needs and pain points to create solutions that are truly valuable."
		},
		{
			icon: ProgressIcon,
			title: 'Clear Progress & Predictability',
			desc: 'We break down every project into transparent, manageable milestones. This gives you full visibility into our progress and ensures a smooth, predictable delivery journey.'
		},
		{
			icon: AgileIcon,
			title: 'Agile Collaboration',
			desc: "We believe the best solutions are built together. Our process is rooted in Agile methodology, prioritizing open communication and close collaboration with you at every step. Your feedback is essential to building a solution that perfectly matches your vision."
		}
	];
</script>

<svelte:head>
	<title>About Us – Applimum</title>
	<meta name="description" content="Learn about Applimum's story, mission, and the guiding principles that drive everything we build." />
</svelte:head>

<!-- Navigation -->
<nav class="flex items-center justify-between px-8 py-6 max-w-7xl mx-auto">
	<a href="/" class="text-2xl font-bold tracking-tight text-brand-dark">APPLIMUM</a>
	<div class="hidden md:flex gap-8 font-medium text-slate-600">
		<a href="/" class="hover:text-brand-heading transition-colors">Home</a>
		<a href="/about" class="text-brand-heading font-semibold transition-colors">About Us</a>
		<a href="/service" class="hover:text-brand-heading transition-colors">Service</a>
		<a href="/case-studies" class="hover:text-brand-heading transition-colors">Case Studies</a>
		<a href="/contact" class="hover:text-brand-heading transition-colors">Contact</a>
	</div>
	<Button class="bg-brand-blue hover:bg-blue-800 text-white rounded-md px-6 cursor-pointer">Get Started</Button>
</nav>

<!-- ===== ABOUT US HERO ===== -->
<section class="relative overflow-hidden bg-gradient-to-br from-white via-brand-light to-white py-28">
	<!-- Decorative dot grid top-left -->
	<div class="absolute top-8 left-8 grid grid-cols-5 gap-3 opacity-40 pointer-events-none" aria-hidden="true">
		{#each {length: 25} as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>
	<!-- Decorative dot grid bottom-right -->
	<div class="absolute bottom-8 right-8 grid grid-cols-5 gap-3 opacity-40 pointer-events-none" aria-hidden="true">
		{#each {length: 25} as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>

	<div class="max-w-5xl mx-auto px-6 text-center relative z-10">
		<h1 class="text-4xl md:text-6xl font-extrabold leading-tight tracking-tight text-brand-heading mb-16">
			We're more than just<br />
			<span class="text-brand-orange">solution providers.</span><br />
			We're <span class="text-brand-orange">partners.</span>
		</h1>

		<!-- Story & Mission Cards -->
		<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
			<!-- Our Story -->
			<div class="bg-white/80 backdrop-blur rounded-2xl border border-slate-100 shadow-sm p-8 text-left">
				<h2 class="text-2xl font-bold text-brand-heading mb-4 text-center">Our Story</h2>
				<p class="text-slate-600 text-sm leading-relaxed mb-3">
					We're driven by the conviction that great work comes from great partnerships. That's why we don't just build and deliver a product;
				</p>
				<p class="text-slate-700 font-bold text-sm leading-relaxed">
					we're driven by the conviction that great work comes from great partnerships. That's why we don't just build and deliver a product; we're committed to building lasting relationships with our clients, providing ongoing support and being a trusted partner for years to come.
				</p>
			</div>

			<!-- Our Mission -->
			<div class="bg-white/80 backdrop-blur rounded-2xl border border-slate-100 shadow-sm p-8 text-left">
				<h2 class="text-2xl font-bold text-brand-heading mb-4 text-center">Our Mission</h2>
				<p class="text-slate-600 text-sm leading-relaxed">
					Is simply to make a real difference for businesses by building software that solves their unique challenges. We believe the right technology isn't just a tool; it's a game-changer that can help a business run smarter, not harder.
				</p>
			</div>
		</div>
	</div>
</section>

<!-- ===== GUIDING PRINCIPLES ===== -->
<section class="py-24 bg-sky-50/60 relative overflow-hidden">
	<!-- Decorative dot grid corners -->
	<div class="absolute top-8 left-8 grid grid-cols-5 gap-3 opacity-30 pointer-events-none" aria-hidden="true">
		{#each {length: 25} as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>
	<div class="absolute bottom-8 right-8 grid grid-cols-5 gap-3 opacity-30 pointer-events-none" aria-hidden="true">
		{#each {length: 25} as _}
			<span class="w-1.5 h-1.5 rounded-full bg-brand-orange inline-block"></span>
		{/each}
	</div>

	<div class="container mx-auto px-6">
		<div class="text-center mb-16">
			<Badge variant="outline" class="text-brand-blue border-brand-blue px-4 py-1 mb-6 rounded-full">Our Methodology</Badge>
			<h2 class="text-4xl md:text-5xl font-extrabold text-brand-heading mb-4">Our Guiding Principles</h2>
			<p class="text-slate-500 max-w-xl mx-auto">These principles are the heartbeat of our company and guide every decision we make.</p>
		</div>

		<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
			{#each principles as principle}
				<div class="bg-white/80 backdrop-blur rounded-2xl border border-slate-100 shadow-sm p-7 hover:shadow-md transition-shadow">
					<principle.icon class="w-14 h-14 mb-5" />
					<h3 class="text-lg font-bold text-brand-heading mb-2">{principle.title}:</h3>
					<p class="text-slate-500 text-sm leading-relaxed">{principle.desc}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<!-- ===== OUR VISION ===== -->
<section class="py-24 bg-white">
	<div class="container mx-auto px-6">
		<div class="max-w-3xl mx-auto bg-white rounded-2xl border border-slate-200 shadow-sm px-12 py-16 text-center">
			<h2 class="text-3xl font-extrabold text-brand-heading mb-6">Our Vision</h2>
			<p class="text-slate-500 leading-relaxed mb-10">
				Our vision is to be the trusted partner businesses turn to for transforming their operations with technology. We want to be known not just for the software we build but for the lasting impact we have on our clients' success.
			</p>
			<div class="flex flex-col sm:flex-row justify-center gap-4">
				<Button class="bg-brand-blue hover:bg-blue-800 text-white px-8 py-5 text-base cursor-pointer">
					Let's Talk →
				</Button>
				<Button variant="outline" class="border-brand-blue text-brand-blue hover:bg-blue-50 px-8 py-5 text-base cursor-pointer">
					View Case Studies
				</Button>
			</div>
		</div>
	</div>
</section>

<!-- Footer -->
<footer class="bg-brand-dark text-slate-300 py-20 text-sm">
	<div class="container mx-auto px-4 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">

		<div class="space-y-6">
			<h3 class="text-2xl font-bold text-white tracking-tight">APPLIMUM</h3>
			<p class="leading-relaxed text-slate-400 max-w-xs">
				Software Engineering and Consulting.<br>
				Building reliable digital solutions for your long-term success.
			</p>
			<div class="pt-2 text-xs text-slate-500">
				&copy; {new Date().getFullYear()} Applimum. All rights reserved.
			</div>
		</div>

		<div>
			<h4 class="font-bold text-brand-heading mb-6 uppercase tracking-wider text-xs">Quick Links</h4>
			<ul class="space-y-4">
				<li><a href="/" class="hover:text-white hover:underline decoration-brand-blue/50 underline-offset-4 transition-all">Home</a></li>
				<li><a href="/about" class="hover:text-white hover:underline decoration-brand-blue/50 underline-offset-4 transition-all">About Us</a></li>
				<li><a href="/#service" class="hover:text-white hover:underline decoration-brand-blue/50 underline-offset-4 transition-all">Services</a></li>
				<li><a href="/#case-studies" class="hover:text-white hover:underline decoration-brand-blue/50 underline-offset-4 transition-all">Case Studies</a></li>
			</ul>
		</div>

		<div>
			<h4 class="font-bold text-brand-heading mb-6 uppercase tracking-wider text-xs">Contact</h4>
			<ul class="space-y-4">
				<li class="flex items-start gap-3 group">
					<Mail class="w-5 h-5 text-slate-500 group-hover:text-brand-blue transition-colors shrink-0" />
					<a href="mailto:info@applimum.com" class="hover:text-brand-blue transition-colors">info@applimum.com</a>
				</li>
				<li class="flex items-start gap-3 group">
					<Phone class="w-5 h-5 text-slate-500 group-hover:text-brand-blue transition-colors shrink-0" />
					<a href="tel:+23409039413344" class="hover:text-brand-blue transition-colors">+234-09039413344</a>
				</li>
			</ul>
		</div>

		<div>
			<h4 class="font-bold text-brand-heading mb-6 uppercase tracking-wider text-xs">Services</h4>
			<ul class="space-y-3 mb-8">
				<li><a href="/#ui-ux" class="hover:text-brand-blue transition-colors">UI/UX Design</a></li>
				<li><a href="/#mobile" class="hover:text-brand-blue transition-colors">Mobile App Development</a></li>
				<li><a href="/#web" class="hover:text-brand-blue transition-colors">Web Development</a></li>
			</ul>

			<h4 class="font-bold text-brand-heading mb-4 uppercase tracking-wider text-xs">Connect</h4>
			<div class="flex gap-4">
				<a href="https://linkedin.com" aria-label="LinkedIn" class="bg-slate-800/50 p-2 rounded-full hover:bg-brand-blue hover:text-white transition-all text-slate-400">
					<Linkedin class="w-4 h-4" />
				</a>
				<a href="https://instagram.com" aria-label="Instagram" class="bg-slate-800/50 p-2 rounded-full hover:bg-brand-orange hover:text-white transition-all text-slate-400">
					<Instagram class="w-4 h-4" />
				</a>
				<a href="https://twitter.com" aria-label="X (Twitter)" class="bg-slate-800/50 p-2 rounded-full hover:bg-slate-700 hover:text-white transition-all text-slate-400">
					<Twitter class="w-4 h-4" />
				</a>
			</div>
		</div>
	</div>

	<div class="container mx-auto px-4 mt-16 pt-8 border-t border-slate-800/50 flex flex-col md:flex-row justify-between items-center text-xs text-slate-500">
		<p class="hidden md:block">Designed with precision.</p>
		<div class="flex gap-6">
			<a href="/privacy" class="hover:text-brand-blue transition-colors">Privacy Policy</a>
			<a href="/terms" class="hover:text-brand-blue transition-colors">Terms of Service</a>
		</div>
	</div>
</footer>
