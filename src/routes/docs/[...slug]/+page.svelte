<script>
	import { page } from '$app/stores';
	console.log($page.params.slug);
	const slugs = $page.params.slug.split('/');
</script>

{#if slugs.length === 1}
	<h3 class="text-center font-semibold text-red-400 text-2xl my-4">
		Viewing docs for feature {slugs[0]}
	</h3>
{:else if slugs.length === 2}
	<h3 class="text-center font-semibold text-red-400 text-2xl my-4">
		Viewing docs for feature {slugs[0]} and concept {slugs[1]}
	</h3>
{/if}
<h1 class="text-center font-semibold text-red-400 text-4xl my-4">Docs Home Page</h1>
