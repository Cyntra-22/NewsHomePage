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
        --button-color: hsl(35, 77%, 62%);
		
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

    .body-container {
            display: flex;
            margin-top: 20px;
        }

    .body-container > div {
            flex: 1; 
        }

    .body-container > div:nth-child(1) {
            flex: 2; 
        }

    .body-container2 {
            display: flex;
            margin-top: 30px;
        }
    .multiple-new-container{
        padding-left: 20px;
        padding-right: 20px;
        background-color: black;
        color: white;
        margin-left: 20px;
    }

</style>

<body>
    <div class="main-container">
        <div class="header">
            <img src="/logo.svg" alt="logo"/>
            <Navigation/>
        </div>
        <div class="body-container">
            <div>
                <New/>
            </div> 
            <div class="multiple-new-container">
                <h1>News</h1>
                <MultipleNew />
                <MultipleNew />
                <MultipleNew />
            </div>   
        </div>
        <div class="body-container2">
            <ThumbNew />
            <ThumbNew/>
            <ThumbNew/>
        </div>
    </div>
    
          
</body>
    

