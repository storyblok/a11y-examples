<script>
	import { storyblokEditable } from '@storyblok/svelte';
	import { getHeadlineTag } from '../utils/getHeadlineTag';

	export let blok;
	export let index;

	const tag = getHeadlineTag(index);
</script>

<svelte:element
	this={tag}
	use:storyblokEditable={blok}
	class="py-32 text-6xl text-[#50b0ae] font-bold text-center"
>
	{blok.headline}</svelte:element
>
