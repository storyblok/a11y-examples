<script>
	import { storyblokEditable, StoryblokComponent } from '@storyblok/svelte';

	export let blok;
</script>

{#key blok}
	<div use:storyblokEditable={blok} class="px-6">
		{#each blok.body as blok, index}
			<StoryblokComponent {blok} {index} />
		{/each}
	</div>
{/key}
