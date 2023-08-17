<template>
    <header>
        <nav class="container">
            <div class="branding">
                <img src="../assets/Vue_Logo_Black.png">
                <h1>Vue Todos</h1>
            </div>
            <ul class="nav-route">
                <Router-link to="/" >Home</Router-link>
                <Router-link to="/about" >About</Router-link>

            </ul>
        </nav>
    </header>
</template>

<script setup>
import {RouterLink} from 'vue-router';
</script>

<style lang="scss" scoped>
header{
    background-color: #f1f1f1;
    nav{
        display: flex;
        align-items: center;
        padding: 25px 26px;

        .branding{
            display: flex;
            align-items: center;
            gap: 8px;
            img{
                max-width: 50px;
            }
            h1{
                font-size: 24px;
            }
        }
        .nav-route{
            display: flex;
            flex: 1;
            justify-content: flex-end;
            gap: 12px;
            list-style: none;

            a{
                text-decoration: none;
                color: inherit;
            }
        }
    }
}

</style>