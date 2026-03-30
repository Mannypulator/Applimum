<script lang="ts">
	import SiteHeader from '$lib/components/SiteHeader.svelte';
</script>

<svelte:head>
	<title>Terms of Service – Applimum</title>
	<meta
		name="description"
		content="Review the basic terms that govern the use of the Applimum website and project enquiries."
	/>
</svelte:head>

<SiteHeader />

<main class="mx-auto max-w-4xl px-6 py-16">
	<div class="rounded-[2rem] border border-slate-200 bg-white p-8 shadow-sm md:p-12">
		<p class="mb-4 text-sm font-semibold uppercase tracking-[0.25em] text-brand-blue">
			Terms of Service
		</p>
		<h1 class="mb-6 text-4xl font-extrabold tracking-tight text-brand-heading">
			Website use and enquiries
		</h1>
		<div class="space-y-6 text-base leading-relaxed text-slate-600">
			<p>
				This website is provided for information about Applimum's software engineering and
				consulting services. Content may be updated over time as our work and offerings
				evolve.
			</p>
			<p>
				Submitting an enquiry through the site does not create a client relationship by
				itself. Any project engagement, pricing, scope, and delivery terms are agreed
				separately in writing.
			</p>
			<p>
				If you have questions about these terms, contact
				<a class="text-brand-blue hover:underline" href="mailto:info@applimum.com">info@applimum.com</a>.
			</p>
		</div>
	</div>
</main>
