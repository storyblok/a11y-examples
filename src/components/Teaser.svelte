<script>
	import { storyblokEditable } from '@storyblok/svelte';

	export let blok;
</script>

<svelte:element
	this={blok.headline_level}
	use:storyblokEditable={blok}
	class="py-32 text-6xl text-[#50b0ae] font-bold text-center"
>
	{blok.headline}
</svelte:element>
