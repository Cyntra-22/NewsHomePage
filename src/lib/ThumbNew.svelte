<script lang="ts">
  import type { Item } from "$lib/types";
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
        margin: 0;
        padding-bottom: 16px;
    }
    p{
        color: var(--text-color);
        font-size: 16px;
        margin: 0;
        padding-bottom: 16px;
    }
    h2{
        font-weight: bold;
        font-size: 25px;
        margin: 0;
        padding-bottom: 16px;

    }
   
    .news-content{
        margin: 0;
        padding: 0;
        padding-left: 20px;
        flex: 2;
        
    }
    .img-container{
        flex: 1;
        
    }
    img{
        width: 130px;
        height: 160px;
    }


    @media (min-width: 300px) and (max-width: 768px ){
        .thumb-new-container{
            padding-top: 20px;
        }
    }

</style>
<div class="thumb-new-container">
        <div class="img-container">
            <img src={item.imageUrl} alt={item.title}/>
        </div>
        <div class="news-content">
                <h1>{item.id}</h1>
                <h2>{item.title}</h2>
                <p>{item.description}</p>
        </div>
</div>
