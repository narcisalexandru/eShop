<template>
    <nav class="nav-container">
        <ul class="nav-menu-left">
            <RouterLink to="/">
                <img class="nav-logo" src="../assets/logo.png" alt="logo">
            </RouterLink>
            <RouterLink 
                to="/store"
                class="nav-link" >
                Store
            </RouterLink>
        </ul>
        <ul class="nav-menu-right">
            <RouterLink 
            to="/cart"
            class="nav-link cart-link">
            <fa icon="cart-shopping"/>
        </RouterLink>
        </ul>
    </nav>
</template>
  
<script lang="ts">
  import { Options, Vue } from 'vue-class-component';
  
  @Options({
    props: {
      msg: String
    }
  })
  export default class Navbar extends Vue {
    msg!: string
  }



</script>
  
<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
    .nav-container {
        display: flex;
        font-family: 'Roboto', sans-serif;
    }

    .nav-menu-left {
        display: flex;
        width: 100%;
        flex-direction: row;
        justify-content: flex-start;
        list-style: none;
        align-items: center;
        gap: 50px;
        padding: 20px;
    }

    .nav-logo {
        display: block;
        width: 80px;
        cursor: pointer;
        transition: all 0.2s ease-in-out;
    }
    .nav-logo:hover {
        -moz-transform: scale(1.1);
        -webkit-transform: scale(1.1);
        -o-transform: scale(1.1);
        -ms-transform: scale(1.1);
        transform: scale(1.1);
    }

    .nav-menu-right {
        display: flex;
        width: 100%;
        flex-direction: row;
        justify-content: flex-end;
        list-style: none;
        align-items: center;
        gap: 50px;
        padding: 20px;
    }
    .nav-link {
        text-decoration: none;
        color: #5a42ec;
        font-size: 18px;
        transition: all 0.2s ease-in-out;
    }
    .nav-link:hover {
        -moz-transform: scale(1.1);
        -webkit-transform: scale(1.1);
        -o-transform: scale(1.1);
        -ms-transform: scale(1.1);
        transform: scale(1.1);
    }
    .nav-link:hover {
        color: #09bbfe;
    }
    .cart-link {
        font-size: 28px;
        /* transition: all 0.2s ease-in-out; */
    }
    .cart-link:hover {
        -moz-transform: scale(1.1);
        -webkit-transform: scale(1.1);
        -o-transform: scale(1.1);
        -ms-transform: scale(1.1);
        transform: scale(1.1);
    }
</style>
  