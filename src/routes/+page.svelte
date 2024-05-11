<script>
  import Navigation from "$lib/Navigation.svelte";
  import New from "$lib/New.svelte";
  import MultipleNew from "$lib/MultipleNew.svelte";
  import ThumbNew from "$lib/ThumbNew.svelte";

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

    .header{
        display: flex;
        justify-content: space-between;
    }

    .multiple-new-container{
        
        color: white;
        
    }

    h1{
        color: var(--title-color);
        font-size: 35px;
    }

    .grid-container {
        display: grid;
        grid-template-columns: auto auto auto;
        gap: 20px;
        margin-top: 20px;
    }

    .grid-container >div{
        padding: 0;
    }

    .item-1{
        grid-column-start: 1;
        grid-column-end: 3;
    }

    .item-2{
        padding: 30px;
        background-color: hsl(240, 100%, 5%);
    }
   

</style>

<body>
    <div class="main-container">
        <div class="header">
            <img src="/logo.svg" alt="logo"/>
            <Navigation/>
        </div>

        <div class="grid-container">
            <div class="item-1">
                <New/>
            </div>
            
            <div class="multiple-new-container">
                <div class="item-2" >
                    <h1>News</h1>
                    <MultipleNew />
                    <MultipleNew />
                    <MultipleNew />
                    
                </div>          
            </div>
            <div class="item-3"><ThumbNew/></div>
            <div class="item-4"><ThumbNew/></div>
            <div class="item-5"><ThumbNew/></div>  
        </div>
    
            
    </div>
   
        
</body>
    



