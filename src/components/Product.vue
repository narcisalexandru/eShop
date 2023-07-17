<template>
    <div class="card">
      <div class="image-container">
        <img :src="product.image" :alt="product.name">
      </div>
      <div class="bottom-container">
        <div class="left">
          <div class="name">{{ product.name }}</div>
          <div class="price">{{ product.price }}</div>
        </div>
        <div class="right">
          <button class="buy-btn"><fa icon="cart-plus" /></button>
        </div>
      </div>
    </div>
  </template>
  
  <script lang="ts">

export default {
  name: 'product',
  props: ['product']
}
  </script>

<style scoped> 
    @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
    *{
        font-family: 'Roboto', sans-serif;
    } 
    .card {
        display: flex;
        justify-content: space-between;
        flex-direction: column;
        width: 200px;
        height: 300px;
        background-color: white;
        box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
        transition: all 0.3s ease-in-out;
    }
    .card:hover {
        -moz-transform: scale(1.03);
        -webkit-transform: scale(1.03);
        -o-transform: scale(1.03);
        -ms-transform: scale(1.03);
        transform: scale(1.03);
    }
    .image-container {
        display: flex;
        width: 100%;
        justify-content: center;
        align-content: flex-start;
    }
    img {
        height: 200px;
        width: 200px;
    }
    .bottom-container {
        display: flex;
        width: 100%;
        height: 70px;
        flex-direction: row;
        justify-content: space-between;
    }
    .right {
        display: flex;
        width: 40%;
        justify-content: center;
        align-items: center;
        background-color: transparent;
        transition: all 0.3s ease-in-out;
    }
    .right:hover {
        background-color: #09bbfe;
    }
    .buy-btn {
        width: 100%;
        height: 100%;
        border: 0px;
        background-color: transparent;
        font-size: 24px;
        color: #5a42ec;
        transition: all 0.3s ease-in-out;

    }
    .buy-btn:hover {
        color: white;
    }
    .left {
        display: flex;
        flex-direction: column;
        width: 60%;
        justify-content: center;
        gap: 2px;
        padding: 15px;
    }
    .name {
        font-size: 24px;
        color: #09bbfe;
    }
    .price {
        text-decoration: none;
    }

</style>