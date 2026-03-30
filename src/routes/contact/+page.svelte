<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter } from '@lucide/svelte';
</script>

<svelte:head>
	<title>Contact – Applimum</title>
	<meta
		name="description"
		content="Get in touch with Applimum. Let's build something amazing together."
	/>
</svelte:head>

<!-- Navigation -->
<nav class="flex items-center justify-between px-8 py-6 max-w-7xl mx-auto">
	<a href="/" class="text-2xl font-bold tracking-tight text-brand-dark">APPLIMUM</a>
	<div class="hidden md:flex gap-8 font-medium text-slate-600">
		<a href="/" class="hover:text-brand-heading transition-colors">Home</a>
		<a href="/about" class="hover:text-brand-heading transition-colors">About Us</a>
		<a href="/service" class="hover:text-brand-heading transition-colors">Service</a>
		<a href="/case-studies" class="hover:text-brand-heading transition-colors">Case Studies</a>
		<a href="/contact" class="text-brand-heading font-semibold transition-colors">Contact</a>
	</div>
	<Button class="bg-brand-blue hover:bg-blue-800 text-white rounded-md px-6 cursor-pointer">
		Get Started
	</Button>
</nav>

<!-- ===== HERO ===== -->
<section class="relative overflow-hidden bg-gradient-to-br from-white via-brand-light to-white pt-16 pb-20">
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
		<!-- Hero heading -->
		<h1 class="text-5xl md:text-7xl font-extrabold leading-tight tracking-tight text-brand-heading mb-16 text-center">
			Let's <span class="text-brand-orange">Build</span> Something<br />
			Amazing Together.
		</h1>

		<!-- Two-column: Contact Details + Contact Form -->
		<div class="grid grid-cols-1 md:grid-cols-2 gap-10 items-start">

			<!-- Left: Contact Details -->
			<div>
				<h2 class="text-2xl font-extrabold text-brand-heading mb-3">Contact Details</h2>
				<p class="text-slate-500 text-sm leading-relaxed mb-8">
					Ready to talk about your project? Give us a call, send an email, or get in touch through the contact form. We're excited to hear your ideas and help you bring them to life.
				</p>

				<ul class="space-y-4 text-sm text-slate-600">
					<li class="flex items-center gap-3">
						<span class="w-8 h-8 rounded-md bg-brand-blue/10 flex items-center justify-center shrink-0">
							<Mail class="w-4 h-4 text-brand-blue" />
						</span>
						<a href="mailto:info@applimum.com" class="hover:text-brand-blue transition-colors">
							info@applimum.com
						</a>
					</li>
					<li class="flex items-center gap-3">
						<span class="w-8 h-8 rounded-md bg-brand-blue/10 flex items-center justify-center shrink-0">
							<Phone class="w-4 h-4 text-brand-blue" />
						</span>
						<a href="tel:+23409039413344" class="hover:text-brand-blue transition-colors">
							+234-09039413344
						</a>
					</li>
					<li class="flex items-center gap-3">
						<span class="w-8 h-8 rounded-md bg-brand-blue/10 flex items-center justify-center shrink-0">
							<Phone class="w-4 h-4 text-brand-blue" />
						</span>
						<a href="tel:+2348076875450" class="hover:text-brand-blue transition-colors">
							08076875450
						</a>
					</li>
					<li class="flex items-center gap-3">
						<span class="w-8 h-8 rounded-md bg-brand-blue/10 flex items-center justify-center shrink-0">
							<Linkedin class="w-4 h-4 text-brand-blue" />
						</span>
						<a href="https://linkedin.com" target="_blank" rel="noreferrer" class="hover:text-brand-blue transition-colors">
							LinkedIn
						</a>
					</li>
					<li class="flex items-center gap-3">
						<span class="w-8 h-8 rounded-md bg-brand-blue/10 flex items-center justify-center shrink-0">
							<Instagram class="w-4 h-4 text-brand-blue" />
						</span>
						<a href="https://instagram.com" target="_blank" rel="noreferrer" class="hover:text-brand-blue transition-colors">
							Instagram
						</a>
					</li>
					<li class="flex items-center gap-3">
						<span class="w-8 h-8 rounded-md bg-brand-blue/10 flex items-center justify-center shrink-0">
							<Twitter class="w-4 h-4 text-brand-blue" />
						</span>
						<a href="https://twitter.com" target="_blank" rel="noreferrer" class="hover:text-brand-blue transition-colors">
							X (formerly Twitter)
						</a>
					</li>
				</ul>
			</div>

			<!-- Right: Contact Form -->
			<div class="bg-white rounded-2xl border border-slate-200 shadow-sm p-8">
				<h2 class="text-2xl font-extrabold text-brand-heading mb-6 text-center">Contact Form</h2>
				<form class="flex flex-col gap-5">
					<div class="flex flex-col gap-1.5">
						<label for="full-name" class="text-sm text-slate-600">Full Name</label>
						<input
							id="full-name"
							type="text"
							placeholder="Enter your name"
							class="w-full border border-slate-200 rounded-lg px-4 py-2.5 text-sm text-slate-800 placeholder:text-slate-400 focus:outline-none focus:ring-2 focus:ring-brand-blue/30 focus:border-brand-blue transition"
						/>
					</div>
					<div class="flex flex-col gap-1.5">
						<label for="email" class="text-sm text-slate-600">Email</label>
						<input
							id="email"
							type="email"
							placeholder="your.email@example.com"
							class="w-full border border-slate-200 rounded-lg px-4 py-2.5 text-sm text-slate-800 placeholder:text-slate-400 focus:outline-none focus:ring-2 focus:ring-brand-blue/30 focus:border-brand-blue transition"
						/>
					</div>
					<div class="flex flex-col gap-1.5">
						<label for="phone" class="text-sm text-slate-600">Phone Number</label>
						<input
							id="phone"
							type="tel"
							placeholder="+234 900 000 0000"
							class="w-full border border-slate-200 rounded-lg px-4 py-2.5 text-sm text-slate-800 placeholder:text-slate-400 focus:outline-none focus:ring-2 focus:ring-brand-blue/30 focus:border-brand-blue transition"
						/>
					</div>
					<div class="flex flex-col gap-1.5">
						<label for="message" class="text-sm text-slate-600">Message</label>
						<textarea
							id="message"
							rows="4"
							placeholder="Tell us about your project..."
							class="w-full border border-slate-200 rounded-lg px-4 py-2.5 text-sm text-slate-800 placeholder:text-slate-400 focus:outline-none focus:ring-2 focus:ring-brand-blue/30 focus:border-brand-blue transition resize-none"
						></textarea>
					</div>
					<Button
						type="submit"
						class="bg-brand-blue hover:bg-blue-800 text-white w-full py-3 text-base cursor-pointer mt-1"
					>
						Send Message
					</Button>
				</form>
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

		<!-- Socials -->
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

	<!-- Bottom bar -->
	<div class="container mx-auto px-8 mt-12 pt-6 border-t border-slate-800/50 flex flex-col md:flex-row justify-between items-center text-xs text-slate-500">
		<p>
			© <strong class="text-slate-300">Applimum {new Date().getFullYear()}.</strong> All rights reserved.
		</p>
		<a href="/privacy" class="hover:text-brand-blue transition-colors mt-2 md:mt-0">Privacy Policy</a>
	</div>
</footer>
