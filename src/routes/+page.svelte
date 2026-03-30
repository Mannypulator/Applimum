<script lang="ts">
	import { Button } from "$lib/components/ui/button";
	import * as Card from "$lib/components/ui/card";
	import { Badge } from "$lib/components/ui/badge";
	import SiteHeader from '$lib/components/SiteHeader.svelte';
	
	// Icons
	import UiUxIcon from "$lib/components/icons/UiUxIcon.svelte";
	import MobileAppIcon from "$lib/components/icons/MobileAppIcon.svelte";
	import WebDevIcon from "$lib/components/icons/WebDevIcon.svelte";
	import ProjectMgmtIcon from "$lib/components/icons/ProjectMgmtIcon.svelte";
	import { Mail, Phone, Linkedin, Instagram, Twitter } from "@lucide/svelte";


	// Data for Services
	const services = [
		{
			icon: UiUxIcon,
			title: "UI/UX Design",
			desc: "We design beautiful and intuitive experiences that customers love."
		},
		{
			icon: MobileAppIcon,
			title: "Mobile App Development",
			desc: "We build powerful, custom apps for iOS and Android."
		},
		{
			icon: WebDevIcon,
			title: "Web Development",
			desc: "We create fast, secure, and scalable web applications."
		},
		{
			icon: ProjectMgmtIcon,
			title: "Project Management",
			desc: "We offer strategic consulting to manage complexity."
		}
	];

	// Data for Process (Timeline)
	const processSteps = [
		{ id: "01", title: "Discovery & Planning", desc: "We start by understanding your business goals and requirements." },
		{ id: "02", title: "Design & Architecture", desc: "Our team designs intuitive user experiences and robust system architecture." },
		{ id: "03", title: "Development & Testing", desc: "We build your solution using best practices with continuous testing." },
		{ id: "04", title: "Deployment & Support", desc: "We deploy your solution seamlessly and provide ongoing support." }
	];
</script>

<SiteHeader />

<section class="relative pt-20 pb-32 overflow-hidden bg-gradient-to-br from-white via-brand-light to-white">
	<div class="absolute inset-0 bg-[url('https://grainy-gradients.vercel.app/noise.svg')] opacity-20"></div>
	
	<div class="max-w-6xl mx-auto text-center relative z-10 px-4">
		<h1 class="text-5xl md:text-7xl font-bold leading-tight tracking-tight text-brand-heading mb-6">
			Building robust <span class="text-brand-orange">digital</span> <br />
			<span class="text-brand-orange">software</span> for your <br />
			<span class="text-brand-orange">long-term success.</span>
		</h1>

		<p class="text-lg text-slate-600 max-w-2xl mx-auto mb-10">
			We <span class="font-bold text-brand-heading">design, build, and scale custom web and mobile solutions.</span>
			We ensure your software is ready to handle all your business growth.
		</p>

		<div class="flex flex-col sm:flex-row justify-center gap-4">
			<Button
				href="/contact"
				size="lg"
				class="bg-brand-blue hover:bg-blue-800 text-white px-8 py-6 text-lg cursor-pointer"
			>
				Start Building
			</Button>
			<Button
				href="/case-studies"
				variant="outline"
				size="lg"
				class="border-brand-blue text-brand-blue hover:bg-blue-50 px-8 py-6 text-lg cursor-pointer"
			>
				View Case Studies
			</Button>
		</div>
	</div>
</section>

<section id="service" class="py-24 bg-white relative">
	<div class="container mx-auto px-4">
		<div class="text-center mb-16">
			<Badge variant="outline" class="text-brand-blue border-brand-blue px-4 py-1 mb-4 rounded-full">Our Expertise</Badge>
			<h2 class="text-4xl font-bold text-brand-heading mb-4">How We Help</h2>
			<p class="text-slate-600">We're a team of experts ready to tackle your toughest challenges</p>
		</div>

		<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
			{#each services as service}
				<Card.Root class="hover:shadow-lg transition-shadow border-slate-100">
					<Card.Header>
						<service.icon class="w-12 h-12 mb-4" />
						<Card.Title class="text-xl font-bold text-brand-heading">{service.title}</Card.Title>
					</Card.Header>
					<Card.Content>
						<p class="text-slate-500 text-sm leading-relaxed">{service.desc}</p>
					</Card.Content>
				</Card.Root>
			{/each}
		</div>
	</div>
</section>

<section class="py-24 bg-sky-50/50">
	<div class="container mx-auto px-4">
		<div class="text-center mb-16">
			<Badge variant="outline" class="text-brand-blue border-brand-blue px-4 py-1 mb-4 rounded-full">Our Methodology</Badge>
			<h2 class="text-4xl font-bold text-brand-blue mb-4">Our Process is your Roadmap</h2>
			<p class="text-slate-600 max-w-2xl mx-auto">We follow a clear, predictable process to ensure high-quality software development and exceptional results.</p>
		</div>

		<div class="relative max-w-4xl mx-auto">
			<div class="absolute left-1/2 transform -translate-x-1/2 h-full w-1 bg-brand-blue hidden md:block"></div>

			<div class="flex flex-col gap-12">
				{#each processSteps as step, i}
					{@const isEven = i % 2 === 0}
					<div class={`flex flex-col md:flex-row items-center ${isEven ? '' : 'md:flex-row-reverse'} relative`}>
						
						<div class="w-full md:w-1/2 px-4">
							<div class="bg-white p-6 rounded-xl shadow-sm borderQl border-slate-100 relative">
								<div class="bg-sky-400 text-white font-bold w-10 h-10 flex items-center justify-center rounded mb-4">
									{step.id}
								</div>
								<h3 class="text-xl font-bold mb-2 text-brand-heading">{step.title}</h3>
								<p class="text-slate-600 text-sm">{step.desc}</p>
							</div>
						</div>

						<div class="hidden md:flex absolute left-1/2 transform -translate-x-1/2 w-4 h-4 bg-brand-blue rounded-full border-4 border-white"></div>
						
						<div class="w-full md:w-1/2 px-4"></div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>

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
				<li><a href="/service" class="hover:text-white hover:underline decoration-brand-blue/50 underline-offset-4 transition-all">Services</a></li>
				<li><a href="/case-studies" class="hover:text-white hover:underline decoration-brand-blue/50 underline-offset-4 transition-all">Case Studies</a></li>
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
				<li><a href="/service" class="hover:text-brand-blue transition-colors">UI/UX Design</a></li>
				<li><a href="/service" class="hover:text-brand-blue transition-colors">Mobile App Development</a></li>
				<li><a href="/service" class="hover:text-brand-blue transition-colors">Web Development</a></li>
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
