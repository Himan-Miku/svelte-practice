<script>
	import { goto } from "$app/navigation"
	const navigate = () => { 
		goto('/products')
	}
</script>

<div class="flex justify-center items-center h-screen">
	<h1 class="text-black text-3xl font-bold">Root Page</h1>
	<button class="bg-blue-400 rounded-xl p-2 font-semibold text-lg text-white ml-6" on:click={navigate}>Place Order</button>
</div>
