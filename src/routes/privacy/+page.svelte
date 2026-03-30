<script lang="ts">
	import SiteHeader from '$lib/components/SiteHeader.svelte';
</script>

<svelte:head>
	<title>Privacy Policy – Applimum</title>
	<meta
		name="description"
		content="Read Applimum's privacy policy and how we handle website and contact information."
	/>
</svelte:head>

<SiteHeader />

<main class="mx-auto max-w-4xl px-6 py-16">
	<div class="rounded-[2rem] border border-slate-200 bg-white p-8 shadow-sm md:p-12">
		<p class="mb-4 text-sm font-semibold uppercase tracking-[0.25em] text-brand-blue">
			Privacy Policy
		</p>
		<h1 class="mb-6 text-4xl font-extrabold tracking-tight text-brand-heading">
			How we handle your information
		</h1>
		<div class="space-y-6 text-base leading-relaxed text-slate-600">
			<p>
				Applimum collects information you choose to share with us, such as your name,
				email address, phone number, and project details when you contact us through this
				website.
			</p>
			<p>
				We use that information only to respond to enquiries, discuss potential projects,
				improve our services, and maintain communication related to ongoing engagements.
			</p>
			<p>
				We do not sell your personal information. If you want your information updated or
				removed, contact us at <a class="text-brand-blue hover:underline" href="mailto:info@applimum.com">info@applimum.com</a>.
			</p>
		</div>
	</div>
</main>
