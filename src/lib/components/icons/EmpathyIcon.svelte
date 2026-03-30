<script lang="ts">
	let { class: className = '' }: { class?: string } = $props();
</script>

<svg class={className} viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
	<rect width="64" height="64" rx="6.4" fill="#FF6B00"/>
	<path d="M32 45s-16-9.5-16-20a10 10 0 0 1 16-8 10 10 0 0 1 16 8c0 10.5-16 20-16 20z" fill="white"/>
</svg>
