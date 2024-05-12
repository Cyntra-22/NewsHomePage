<script lang="ts">
  import New from "$lib/New.svelte";
  import MultipleNew from "$lib/MultipleNew.svelte";
  import ThumbNew from "$lib/ThumbNew.svelte";
  import { writable } from 'svelte/store';

  const newsData = writable([
    { 
      id: "01",
      title: "Reviving Retro PCs", 
      description: "What happens when old PCs are given modern upgrades?", 
      image: "/image-retro-pcs"
    },
    { 
      id: "02",
      title: "Top 10 Laptops of 2022", 
      description: "Our best picks for various needs and budgets. ", 
      image: "/image-top-laptops"
    },
    { 
      id: "03",
      title: "The Growth of Gaming", 
      description: "How the pandemic has sparked fresh opportunities.", 
      image: "/static/image-gaming-growth.jpg"
    },
      
  ]);

</script>
<style>
    
   

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
            <div class="item-3"><ThumbNew /></div>
            <div class="item-4"><ThumbNew /></div>
            <div class="item-5"><ThumbNew /></div>  
</div>
    
            

   






    



