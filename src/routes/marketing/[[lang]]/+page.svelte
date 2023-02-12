<script>
	import { page } from '$app/stores';
	const greetings = {
		en: 'Hello!',
		sp: 'Hola!',
		fr: 'Bonjour'
	};
	const { lang = 'en' } = $page.params;
	const greeting = greetings[lang];
	console.log(greeting);
</script>

{#if greeting === undefined}
	<div class="flex justify-center items-center">
		<h1
			class="text-center font-bold text-white p-4 inline-block rounded-xl bg-red-400 text-4xl my-4"
		>
			Sorry This Language Is Not Supported
		</h1>
	</div>
{:else}
	<h1 class="text-center font-bold text-blue-400 text-4xl my-4">{greeting}</h1>
{/if}
