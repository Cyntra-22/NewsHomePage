<script lang="ts">
    import {page} from "$app/stores";

    $: routeId = $page.route.id;
    
</script>

<style>
    .nav-container{
        width: 80%;
        margin: 30px auto;
        padding: 10px;
    }
        .header{
        display: flex;
        justify-content: space-between;
    }
       
        ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        overflow: hidden;
        }

        li {
        float: left;
        }

        li a {
        display: block;
        color: black;
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
        cursor: pointer;
        }

        li a:hover {
        color: var(--button-color);
        }
        
        button{
            border: none;
            background-color: transparent;
            cursor: pointer;
            padding-top: 15px;
        }

        .mobile-nav{
            display: none;
        }

        .active{
            color: var(--button-color);
        }
        
        @media (min-width:300px ) and (max-width: 600px){
           
            .mobile-nav{
                display: block;
            }
            .desktop-nav > ul{
                display: none;
            }
           .mobile-nav>ul {
            display: none;
           }
        }
</style>

<div class="nav-container">  
    <div class="header">
        <div>
            <img src="/logo.svg" alt="logo"/>
        </div>
        <div class="desktop-nav">
                <ul >
                    <li><a class:active = {routeId ==="/"} href="/">Home</a></li>
                    <li><a class:active = {routeId ==="/about"} href="/newnav" >News</a></li>
                    <li><a class:active = {routeId ==="/popular"} href="/popular" >Popular</a></li>
                    <li><a class:active = {routeId ==="/trending"} href="/trending" >Trending</a></li>
                    <li><a class:active = {routeId ==="/categories"} href="/categories" >Categories</a></li>
                </ul>          
        </div> 
        <div class="mobile-nav">
            <button ><img src="/icon-menu.svg" alt="nav icon"></button> 
                <ul >
                    <li><a href="/">Home</a></li>
                    <li><a href="/newnav" >News</a></li>
                    <li><a href="/popular" >Popular</a></li>
                    <li><a href="/trending" >Trending</a></li>
                    <li><a href="/categories" >Categories</a></li>
                </ul>          
        </div> 
        
    </div>
</div> 


<!--

<script lang="ts">
    import { page } from "$app/stores";
    import { writable } from "svelte/store";
  
    const isMobileMenuOpen = writable(false);

    function toggleMobileMenu() {
        isMobileMenuOpen.update(value => !value);
    }

    console.log(page);
</script>

<style>
    .nav-container {
        width: 80%;
        margin: 30px auto;
        padding: 10px;
    }

    .header {
        display: flex;
        justify-content: space-between;
    }

    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        overflow: hidden;
    }

    li {
        float: left;
    }

    li a {
        display: block;
        color: black;
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
        cursor: pointer;
    }

    li a:hover {
        color: var(--button-color);
    }

    button {
        border: none;
        background-color: transparent;
        cursor: pointer;
        padding-top: 15px;
    }

    .mobile-nav {
        display: none;
    }

    @media (min-width: 300px) and (max-width: 600px) {
        .mobile-nav {
            display: block;
        }

        .desktop-nav > ul {
            display: none;
        }

        .mobile-nav > ul {
            display: none;
            flex-direction: column;
        }

        .mobile-nav ul li {
            float: none;
        }
    }
</style>

<div class="nav-container">
    <div class="header">
        <div>
            <img src="/logo.svg" alt="logo" />
        </div>
        <div class="desktop-nav">
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/newnav">News</a></li>
                <li><a href="/popular">Popular</a></li>
                <li><a href="/trending">Trending</a></li>
                <li><a href="/categories">Categories</a></li>
            </ul>
        </div>
        <div class="mobile-nav">
            <button on:click={toggleMobileMenu}><img src="/icon-menu.svg" alt="nav icon"></button>
            {#if $isMobileMenuOpen}
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/newnav">News</a></li>
                <li><a href="/popular">Popular</a></li>
                <li><a href="/trending">Trending</a></li>
                <li><a href="/categories">Categories</a></li>
            </ul>
            {/if}
        </div>
    </div>
</div>

-->
