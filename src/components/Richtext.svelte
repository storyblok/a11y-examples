<script>
	import { storyblokEditable, renderRichText } from '@storyblok/svelte';

	export let blok;
	$: resolvedRichText = renderRichText(blok.text);
</script>

<div use:storyblokEditable={blok} class="prose py-12">
	{@html resolvedRichText}
</div>
