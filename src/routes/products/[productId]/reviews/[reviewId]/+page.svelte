<script>
    import { page } from "$app/stores"
    const { productId, reviewId } = $page.params
</script>

<div>
    <h3 class="text-red-500 text-center text-3xl font-bold">Review {reviewId} of Product {productId} </h3>
</div>