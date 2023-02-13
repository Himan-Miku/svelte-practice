<script>
    import { goto } from "$app/navigation"
    const handleClick1 = () => {
        goto('/products/product1')
    }
    const handleClick2 = () => {
        goto('/products/product2')
    }
    const handleClick3 = () => {
        goto('/products/product3')
    }
</script>

<h1 class="text-4xl my-4 text-center text-blue-500 font-bold">Products page</h1>
<ul class="flex gap-6 ml-8">
    <li on:click={handleClick1} class="bg-red-400 rounded-md p-2 text-black font-medium"> Product 1 </li>
    <li on:click={handleClick2} class="bg-red-400 rounded-md p-2 text-black font-medium"> Product 2 </li>
    <li on:click={handleClick3} class="bg-red-400 rounded-md p-2 text-black font-medium"> Product 3 </li>
</ul>