<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Mail, Phone, Linkedin, Instagram, Twitter, ArrowLeft } from '@lucide/svelte';
	import SiteHeader from '$lib/components/SiteHeader.svelte';
</script>

<svelte:head>
	<title>SwiftMove Case Study - Applimum</title>
	<meta
		name="description"
		content="See how Applimum designed a realtime logistics tracking experience for SwiftMove."
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

	<div class="relative mb-20 overflow-hidden rounded-[2rem] bg-linear-to-br from-slate-900 via-slate-800 to-cyan-700 p-10 text-white md:p-16">
		<div class="grid gap-10 md:grid-cols-2 md:items-center">
			<div class="z-10 flex flex-col items-start gap-6">
				<div class="rounded-full border border-white/20 bg-white/10 px-4 py-2 text-sm font-semibold uppercase tracking-[0.25em]">
					Logistics Product Design
				</div>
				<h1 class="text-4xl font-extrabold leading-tight md:text-5xl">
					SwiftMove: Logistics Tracking App
				</h1>
				<p class="max-w-xl text-lg leading-relaxed text-white/85">
					We designed a clearer shipment experience for customers and operations teams so
					everyone could track delivery progress, reduce uncertainty, and react faster in the
					middle of active movement.
				</p>
			</div>

			<div class="grid gap-4 rounded-[1.75rem] border border-white/15 bg-white/8 p-6 backdrop-blur-sm">
				<div class="rounded-[1.5rem] border border-white/15 bg-slate-950/25 p-5">
					<p class="text-sm font-semibold uppercase tracking-[0.2em] text-white/60">
						Product focus
					</p>
					<ul class="mt-4 space-y-3 text-sm text-white/80">
						<li>Realtime shipment visibility</li>
						<li>Driver and dispatcher coordination</li>
						<li>Customer notifications at critical moments</li>
					</ul>
				</div>
				<div class="grid grid-cols-2 gap-4">
					<div class="rounded-2xl bg-white/12 p-5">
						<p class="text-xs font-semibold uppercase tracking-[0.25em] text-white/65">
							Tracking
						</p>
						<p class="mt-3 text-3xl font-extrabold">Live</p>
						<p class="mt-2 text-sm text-white/75">Visibility from dispatch to dropoff</p>
					</div>
					<div class="rounded-2xl bg-white/12 p-5">
						<p class="text-xs font-semibold uppercase tracking-[0.25em] text-white/65">
							Support
						</p>
						<p class="mt-3 text-3xl font-extrabold">Less</p>
						<p class="mt-2 text-sm text-white/75">Customer uncertainty and status chasing</p>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="mb-20 grid gap-12 md:grid-cols-2 md:items-start">
		<div class="rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">Client Overview</h2>
			<p class="text-lg leading-relaxed text-slate-600">
				SwiftMove needed a customer-facing tracking experience and a more reliable operational
				workflow for shipments in motion. Their goal was to make delivery progress legible at a
				glance while giving internal teams clearer decision support.
			</p>
		</div>
		<div class="rounded-2xl border border-slate-200 bg-slate-50 p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">The Challenge</h2>
			<ul class="list-disc space-y-3 pl-5 leading-relaxed text-slate-600">
				<li>Customers had limited visibility once a shipment was in transit.</li>
				<li>Dispatchers and drivers relied on fragmented updates.</li>
				<li>Support teams spent too much time answering status questions.</li>
				<li>The mobile experience needed to work well in time-sensitive contexts.</li>
			</ul>
		</div>
	</div>

	<div class="mb-20 grid gap-12 md:grid-cols-2 md:items-start">
		<div class="rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">Our Approach</h2>
			<div class="space-y-6 text-slate-600">
				<div>
					<p class="font-semibold text-slate-800">1. Journey mapping</p>
					<p class="mt-2 leading-relaxed">
						We mapped how customers, dispatchers, and drivers each interpret shipment state so
						the interface could support all three viewpoints without overwhelming any one of them.
					</p>
				</div>
				<div>
					<p class="font-semibold text-slate-800">2. Mobile-first interaction design</p>
					<p class="mt-2 leading-relaxed">
						We focused on status clarity, alert timing, and quick scanning so the most important
						updates stayed visible on smaller screens and under time pressure.
					</p>
				</div>
				<div>
					<p class="font-semibold text-slate-800">3. Operational alignment</p>
					<p class="mt-2 leading-relaxed">
						We shaped the product around dispatch workflows and notification triggers so the
						experience was useful operationally, not just visually polished.
					</p>
				</div>
			</div>
		</div>
		<div class="rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
			<h2 class="mb-6 text-2xl font-bold text-brand-heading">The Solution</h2>
			<ul class="space-y-4 text-slate-600">
				<li><strong class="text-slate-800">Realtime tracking flow:</strong> clear progress states from pickup through delivery.</li>
				<li><strong class="text-slate-800">Status notifications:</strong> updates at the moments customers care about most.</li>
				<li><strong class="text-slate-800">Driver workflow support:</strong> better visibility for movement, updates, and exceptions.</li>
				<li><strong class="text-slate-800">Operations visibility:</strong> a stronger base for dispatch and support coordination.</li>
			</ul>
		</div>
	</div>

	<div class="mb-20 rounded-2xl border border-slate-200 bg-white p-8 shadow-sm md:p-10">
		<h2 class="mb-6 text-2xl font-bold text-brand-heading">The Impact</h2>
		<div class="grid gap-4 md:grid-cols-2">
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Clearer</p>
				<p class="mt-2 text-slate-600">Shipment visibility for customers waiting on delivery.</p>
			</div>
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Faster</p>
				<p class="mt-2 text-slate-600">Issue escalation for operations teams handling live movement.</p>
			</div>
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Lower</p>
				<p class="mt-2 text-slate-600">Support burden caused by manual status requests and uncertainty.</p>
			</div>
			<div class="rounded-2xl bg-sky-50 p-6">
				<p class="text-3xl font-extrabold text-brand-heading">Stronger</p>
				<p class="mt-2 text-slate-600">Mobile experience for customers, drivers, and dispatch teams.</p>
			</div>
		</div>
	</div>

	<div class="relative overflow-hidden rounded-[2rem] bg-brand-light p-12 text-center">
		<h2 class="relative z-10 mb-6 text-4xl font-extrabold text-brand-dark md:text-5xl">
			Building logistics software with more clarity?
		</h2>
		<p class="relative z-10 mx-auto mb-10 max-w-3xl text-lg leading-relaxed text-slate-600">
			We can help shape the customer experience, operational workflow, and interface system
			needed for realtime logistics products.
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
