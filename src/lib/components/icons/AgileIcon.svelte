<script lang="ts">
	let { class: className = '' }: { class?: string } = $props();
</script>

<svg class={className} viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
	<rect width="64" height="64" rx="6.4" fill="#FF6B00"/>
	<circle cx="24" cy="26" r="5" fill="white"/>
	<circle cx="40" cy="26" r="5" fill="white"/>
	<path d="M14 44c0-5.5 4.5-10 10-10h4c5.5 0 10 4.5 10 10H14z" fill="white"/>
	<path d="M36 44c0-5.5 4.5-10 10-10h4c0 5.5-4.5 10-10 10h-4z" fill="white"/>
</svg>
