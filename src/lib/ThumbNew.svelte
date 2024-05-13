<script lang="ts">
  import type { Item } from "./types";
  export let item: Item;
</script>
<style>
    .thumb-new-container{
        display: flex;
       
    }
    h1{
        color: var(--font-color);
        font-size: 28px;
        font-weight: bold;
    }
    p{
        color: var(--text-color);
        font-size: 16px;
    }
    h2{
        font-weight: bold;
        font-size: 25px;
    }
   
    .news-content{
        padding: 20px;
    }


</style>
    <div class="thumb-new-container">
        <div>
            <img src={item.imageUrl} alt={item.title}/>
        </div>
        <div class="news-content">
            <div>
                <h1>{item.id}</h1>
                <h2>{item.title}</h2>
                <p>{item.description}</p>
            </div>
        </div>
    </div>
