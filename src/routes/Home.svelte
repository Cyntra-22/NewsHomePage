<script lang="ts">
  import New from "$lib/New.svelte";
  import MultipleNew from "$lib/MultipleNew.svelte";
  import ThumbNew from "$lib/ThumbNew.svelte";
  import {items} from "$lib/data";
  import type {Item} from "$lib/types";

  const myItems: Item[] = items;
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
            {#each myItems as item(item.id)}
              <ThumbNew {item} />
            {/each}
</div>
    
            

   






    



