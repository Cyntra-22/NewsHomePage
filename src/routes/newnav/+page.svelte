<script lang="ts">
    import ThumbNew from "$lib/ThumbNew.svelte";
    import NavNew from "$lib/NavNew.svelte";
    import type {Item} from "$lib/types";
    import {items} from "$lib/data";

    const  navNews:Item[] = items;
</script>
<style>
    .new-container{
        display: flex;
        width: 100%;
        justify-content: space-between;

    }
    img{
        width: 100%;    
    }
    .img-container{
        margin-right: 20px;
    }

    @media (min-width: 300px) and (max-width: 768px ){
        .new-container{
            display: block;
        }
    }
    
</style>

<div class="new-container">
    <div class="img-container">
        <div >
            <img src="/image-web-3-desktop.jpg" alt="new title"/>
            <h1>Tech titans clash: Inside the US-China battle for chip market dominance</h1>
        </div>
        <div class="new-container ">
            <NavNew/>
            <NavNew/>
        </div>
        <div class="new-container ">
            <NavNew/>
            <NavNew/>
        </div>
        
    </div>
    <div>
        {#each navNews as item(item.id)}
            <div>
            <ThumbNew {item} />
            </div>        
        {/each}
        {#each navNews as item(item.id)}
            <div>
            <ThumbNew {item} />
            </div>        
        {/each} 
    </div>
</div>