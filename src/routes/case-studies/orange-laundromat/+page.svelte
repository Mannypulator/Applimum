<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter, ArrowLeft } from '@lucide/svelte';
</script>

<svelte:head>
	<title>Orange Laundromat Case Study – Applimum</title>
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

<main class="max-w-6xl mx-auto px-6 pb-24">
	<!-- Back Button -->
	<div class="mb-8 mt-4">
		<a href="/case-studies" class="inline-flex flex-row items-center gap-2 border border-brand-blue/30 text-brand-blue hover:bg-brand-blue/5 px-4 py-2 rounded-md font-semibold text-sm transition-colors">
			<ArrowLeft class="w-4 h-4" />
			Back
		</a>
	</div>

	<!-- Hero Banner -->
	<div class="bg-[#E87A1E] rounded-[2rem] p-10 md:p-16 flex flex-col md:flex-row items-center gap-10 text-white mb-20 relative overflow-hidden">
		<div class="md:w-1/2 flex flex-col items-start gap-6 z-10">
			<div class="flex items-center gap-3">
				<div class="w-12 h-12 rounded-full bg-white/20 flex items-center justify-center">
					<!-- logo mark -->
					<svg class="w-6 h-6 text-white" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"></circle><path d="m12 2 4 10H8z"></path><path d="M12 22V12"></path></svg>
				</div>
				<span class="text-2xl font-bold tracking-tight">Orange <br/><span class="font-medium">Laundromat</span></span>
			</div>
			<h1 class="text-4xl md:text-5xl font-extrabold leading-tight">Orange Laundromat:<br/> Reinventing Laundry<br/> Convenience</h1>
		</div>
		<div class="md:w-1/2 relative h-64 md:h-[400px] w-full rounded-xl flex items-center justify-center z-10">
			<img src="/orange-laudromat.svg" alt="Orange Laundromat screens" class="w-full h-full object-cover md:object-contain drop-shadow-2xl" />
		</div>
	</div>

	<!-- Client Overview & Mobile Apps -->
	<div class="grid grid-cols-1 md:grid-cols-2 gap-12 mb-20 items-center">
		<div class="border border-slate-200 rounded-2xl p-8 md:p-10 shadow-sm bg-white self-start">
			<h2 class="text-2xl font-bold text-[#8B5CF6] mb-6">Client Overview</h2>
			<p class="text-slate-600 leading-relaxed text-lg">
				Orange Laundromat is a tech-driven laundry startup on a mission to make washing and dry-cleaning effortless. They envisioned a platform that allows users to book laundry services, track orders, and enjoy doorstep pickup and delivery – transforming a traditionally stressful chore into a seamless digital experience.
			</p>
		</div>
		<div class="h-[450px] bg-slate-50/50 rounded-2xl flex items-center justify-center border border-slate-200 overflow-hidden">
			<img src="/door-step.svg" alt="App Feature" class="w-full h-full object-cover" />
		</div>
	</div>

	<!-- The Challenge & Laptop -->
	<div class="grid grid-cols-1 md:grid-cols-2 gap-12 mb-20 items-center">
		<div class="h-[450px] bg-slate-50/50 rounded-2xl flex items-center justify-center border border-slate-200 overflow-hidden order-2 md:order-1 p-6">
			<img src="/laptop-challenge.svg" alt="Laptop Challenge" class="w-full h-full object-contain drop-shadow-xl" />
		</div>
		<div class="border border-slate-200 rounded-2xl p-8 md:p-10 shadow-sm bg-white order-1 md:order-2 self-start">
			<h2 class="text-2xl font-bold text-[#8B5CF6] mb-6">The Challenge</h2>
			<p class="text-slate-600 leading-relaxed mb-4">
				Before reaching out to us, Orange Laundromat had a clear vision but were unsure of the product direction.
			</p>
			<p class="text-slate-600 font-medium mb-3">They needed:</p>
			<ul class="list-disc pl-5 text-slate-600 space-y-3 leading-relaxed mb-4">
				<li>A website and mobile app experience that was simple, clean, and engaging.</li>
				<li>A user flow that minimized friction in booking pickups and deliveries.</li>
				<li>A way to integrate subscription plans, wallet payments, and real-time order tracking.</li>
				<li>A visual identity that reflected freshness, care, and trust.</li>
			</ul>
			<p class="text-slate-600 leading-relaxed">
				Essentially, they wanted to create "the Uber of laundry" - a full-service solution that modern users could rely on daily.
			</p>
		</div>
	</div>

	<!-- Our Approach & Laptop Approach SVG -->
	<div class="grid grid-cols-1 md:grid-cols-2 gap-12 mb-20 items-center">
		<div class="border border-slate-200 rounded-2xl p-8 md:p-10 shadow-sm bg-white self-start">
			<h2 class="text-2xl font-bold text-[#8B5CF6] mb-6">Our Approach</h2>
			<p class="text-slate-600 leading-relaxed mb-4">
				We began by defining the user journey from first-time signup to repeat orders. Our design process followed a lean product design framework:
			</p>
			<p class="text-slate-800 font-semibold mb-2">1. Discovery & Research</p>
			<p class="text-slate-600 leading-relaxed mb-4">
				We explored user pain points with existing laundry services and identified opportunities around speed and transparency, pickup scheduling flexibility, and subscription convenience.
			</p>
			
			<p class="text-slate-800 font-semibold mb-2">2. Experience Mapping</p>
			<p class="text-slate-600 leading-relaxed mb-4">
				We mapped two primary user types: one-time customers needing fast service, and subscribers seeking ongoing convenience and savings. Each flow was optimized to reduce the time to book to under 30 seconds.
			</p>

			<p class="text-slate-800 font-semibold mb-2">3. UI Design & Prototyping</p>
			<p class="text-slate-600 leading-relaxed mb-2">
				We created a fresh, modern visual system that blends simplicity and warmth:
			</p>
			<ul class="list-disc pl-5 text-slate-600 space-y-2 leading-relaxed">
				<li>A clean white and orange color palette evoking freshness and energy.</li>
				<li>Friendly iconography and rounded shapes to communicate ease.</li>
				<li>Contextual microcopy guiding users at every step.</li>
			</ul>
		</div>
		<div class="flex items-center justify-center">
			<img src="/laptop-approach.svg" alt="Laptop Approach Mockup" class="w-full max-w-[511px] drop-shadow-xl" />
		</div>
	</div>

	<!-- The Solution -->
	<div class="mb-12">
		<div class="border border-slate-200 rounded-2xl p-8 md:p-10 shadow-sm bg-white w-full max-w-4xl mx-auto">
			<h2 class="text-2xl font-bold text-[#8B5CF6] mb-6">The Solution</h2>
			<p class="text-slate-600 leading-relaxed mb-6">
				The final product delivered a smooth, end-to-end laundry experience:
			</p>
			<ul class="space-y-4 text-slate-600">
				<li>
					<strong class="text-slate-800">Effortless Onboarding:</strong> A 3-step onboarding that introduces users to scheduling, convenience, and affordable plans.
				</li>
				<li>
					<strong class="text-slate-800">Smart Booking Flow:</strong> Users can select services (Wash & Iron, Dry Cleaning, etc.), choose pickup time, and specify delivery speed.
				</li>
				<li>
					<strong class="text-slate-800">Seamless Payment Integration:</strong> Supports wallet, card, and bank transfers with auto-calculation for plan.
				</li>
				<li>
					<strong class="text-slate-800">Real-Time Order Tracking:</strong> Users get notified when clothes are picked up, cleaned, and delivered.
				</li>
				<li>
					<strong class="text-slate-800">Subscription & Loyalty Programs:</strong> Designed for recurring engagement with incentives and point-based rewards.
				</li>
				<li>
					<strong class="text-slate-800">Admin Dashboard:</strong> For managing orders, riders, and subscription analytics.
				</li>
			</ul>
		</div>
	</div>

	<!-- UI UX SVG -->
	<div class="mb-20 w-full flex justify-center">
		<img src="/ui-ux.svg" alt="UI/UX Screens Showcase" class="w-full object-contain" />
	</div>

	<!-- The Impact -->
	<div class="mb-20">
		<div class="border border-slate-200 rounded-2xl p-8 md:p-10 shadow-sm bg-white w-full max-w-4xl mx-auto">
			<h2 class="text-2xl font-bold text-[#8B5CF6] mb-6">The Impact</h2>
			<p class="text-slate-600 leading-relaxed mb-4">
				Within weeks of launch, Orange Laundromat reported:
			</p>
			<ul class="space-y-3 text-slate-600 leading-relaxed">
				<li class="flex items-start gap-2">
					<span>🚀</span>
					<span>65% faster booking times</span>
				</li>
				<li class="flex items-start gap-2">
					<span>🔄</span>
					<span>Increased customer retention via subscription plans</span>
				</li>
				<li class="flex items-start gap-2">
					<span>📈</span>
					<span>A 40% boost in repeat usage within the first quarter</span>
				</li>
				<li class="flex items-start gap-2">
					<span>⭐</span>
					<span>Positive feedback highlighting convenience and transparency</span>
				</li>
			</ul>
		</div>
	</div>

	<!-- Join Our Mission -->
	<div class="bg-brand-light flex flex-col items-center justify-center rounded-[2rem] p-12 text-center relative overflow-hidden">
		<!-- Decorative small dots -->
		<div class="absolute inset-0 opacity-40 pointer-events-none" aria-hidden="true">
			<div class="absolute top-[20%] left-[20%] w-1.5 h-1.5 bg-brand-orange rounded-full"></div>
			<div class="absolute top-[40%] left-[10%] w-1.5 h-1.5 bg-brand-orange rounded-full"></div>
			<div class="absolute top-[70%] left-[25%] w-1.5 h-1.5 bg-brand-orange rounded-full"></div>
			<div class="absolute top-[30%] right-[20%] w-1.5 h-1.5 bg-brand-orange rounded-full"></div>
			<div class="absolute top-[60%] right-[15%] w-1.5 h-1.5 bg-brand-orange rounded-full"></div>
			<div class="absolute top-[80%] right-[30%] w-1.5 h-1.5 bg-brand-orange rounded-full"></div>
		</div>

		<h2 class="text-4xl md:text-5xl font-extrabold text-brand-dark mb-6 relative z-10 w-full">Join Our Mission</h2>
		<p class="text-slate-600 text-lg max-w-3xl mx-auto mb-10 relative z-10 leading-relaxed w-full">
			Ready to build the future of digital experiences for your customers? Partner with Applimum, the web development agency trusted by forward-thinking brands to craft powerful, scalable, and user-focused products. Let's turn your vision into a product that drives results.
		</p>
		<Button class="bg-brand-blue hover:bg-blue-800 text-white rounded-md px-8 py-6 text-lg cursor-pointer relative z-10 font-semibold shadow-lg shadow-brand-blue/20">
			Start Building Today →
		</Button>
	</div>
</main>

<!-- ===== FOOTER ===== -->
<footer class="bg-brand-dark text-slate-300 py-16 text-sm">
	<div class="container mx-auto px-8 grid grid-cols-1 md:grid-cols-4 gap-10 w-full max-w-7xl">
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
				<li><a href="/case-studies" class="hover:text-white transition-colors">Case Studies</a></li>
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

	<div class="container mx-auto px-8 mt-12 pt-6 border-t border-slate-800/50 flex flex-col md:flex-row justify-between items-center text-xs text-slate-500 max-w-7xl">
		<p>© <strong class="text-slate-300">Applimum {new Date().getFullYear()}.</strong> All rights reserved.</p>
		<a href="/privacy" class="hover:text-brand-blue transition-colors mt-2 md:mt-0">Privacy Policy</a>
	</div>
</footer>
