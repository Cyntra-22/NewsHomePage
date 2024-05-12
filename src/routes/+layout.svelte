<script lang="ts">
    import Navbar from "./Navbar.svelte";
</script>
<style>
    :root{
		--font-color: hsl(233, 8%, 79%);
        --text-color: hsl(236, 13%, 42%);
		--font: 'Inter', sans-serif;
        --title-color: hsl(35, 77%, 62%);
        --button-color: hsl(5, 85%, 63%);
		
	}

	:global(body){
		
		margin: 0 auto;
		font-family: var(--font); 
		 
	}
     .main-container{
        width: 80%;
        margin: 30px auto;
        padding: 10px;

    }
</style>
<Navbar/>
<body>
    <div class="main-container">
        <slot/>
    </div>  
</body>

