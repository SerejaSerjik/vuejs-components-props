<template>
    <div class="product">
        <h2>Product Detail</h2>
        <form>
        <div>
            <label for="title">Title</label>
            <span>{{product.title}}</span>
        </div>
        <div>
            <label for="price">Price</label>
            <span>${{product.price}}</span>
        </div>
        <div>
            <label for="qt">Quantity</label>
            <span>{{product.qt}}</span>
        </div>
        </form>    
    </div>
</template>

<script>

    export default {  
        props: {
            product: {
                type: Object,
                required: true
            }
        },
        data(){
            return {
                //product: {}
            }
        },   
    }    
</script>

<style scoped>
    .product {
        width: 500px;
        border: 1px solid red;
        border-radius: 10px;
        margin: 10px;
        padding: 10px;  
    }
</style>