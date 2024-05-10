<script>
  import Navigation from "$lib/Navigation.svelte";


</script>
<style>
    :root{
		--font-color: hsl(233, 8%, 79%);
        --text-color: hsl(236, 13%, 42%);
		--font: 'Inter', sans-serif;
        --button-color: hsl(35, 77%, 62%);
		
	}

	:global(body){
		
		margin: 0 auto;
		font-family: var(--font); 
		 
	}
    .main-container{
        width: 80%;
        background-color: aqua;
        margin: 0 auto;

    }

    .header{
        display: flex;
        justify-content: space-between;
    }

</style>

<body>
    <div class="main-container">
        <div class="header">
            <img src="/logo.svg" alt="logo"/>
            <Navigation/>
        </div>
    </div>
    
          
</body>
    

