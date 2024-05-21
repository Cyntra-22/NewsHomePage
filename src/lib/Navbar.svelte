<script lang="ts">
    import { page } from "$app/stores";
    import { writable } from "svelte/store";

    $: routeId = $page.route.id;
    
    const isNavOpen = writable(false);

    function toggleNav() {
        isNavOpen.update(n => !n);
    }
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
        align-items: center;
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
    .active {
        color: var(--button-color);
    }
    @media (min-width: 300px) and (max-width: 600px) {
        .mobile-nav {
            display: block;
        }
        .desktop-nav > ul {
            display: none;
        }
        .mobile-nav > div {
            display: none;
        }
        .mobile-nav div.open {
            display: block;
            position: fixed;
            right: 0;
            top: 0;
            width: 250px;
            height: 100%;
            background: white;
            box-shadow: -1px 0 5px rgba(0,0,0,0.5);
            z-index: 1000;
        }
        
        .mobile-nav li {
            float: none;
            text-align: left;
        }
        .icon-style {
            display: flex;
            justify-content: flex-end;
            padding-left: 200px;
            padding-bottom: 25px;
            
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
                <li><a class:active={routeId === "/"} href="/">Home</a></li>
                <li><a class:active={routeId === "/newnav"} href="/newnav">News</a></li>
                <li><a class:active={routeId === "/popular"} href="/popular">Popular</a></li>
                <li><a class:active={routeId === "/trending"} href="/trending">Trending</a></li>
                <li><a class:active={routeId === "/categories"} href="/categories">Categories</a></li>
            </ul>
        </div>
        <div class="mobile-nav">
            <button on:click={toggleNav}>
                <img src={$isNavOpen ? "/icon-close.svg" : "/icon-menu.svg"} alt="nav icon" />
            </button>
            <div class:open={$isNavOpen}>
                <button on:click={toggleNav} class="icon-style">
                    <img src="/icon-menu-close.svg" alt="nav close icon" />
                </button>
                <ul>
                    <li><a class:active={routeId === "/"} href="/">Home</a></li>
                    <li><a class:active={routeId === "/newnav"} href="/newnav">News</a></li>
                    <li><a class:active={routeId === "/popular"} href="/popular">Popular</a></li>
                    <li><a class:active={routeId === "/trending"} href="/trending">Trending</a></li>
                    <li><a class:active={routeId === "/categories"} href="/categories">Categories</a></li>
                </ul>
            </div>
        </div>
    </div>
</div>





