<script lang="ts">
    export let newsData:{id:string, title:string, description:string, image:string}[];
    export let id:string;

     $: News = $newsData.filter(news => news.id === id) as { id: string, title: string, description: string, image: string }[];

</script>
<style>
    .thumb-new-container{
        display: flex;
        margin-top: 15px;
        
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
{#each News as news}
    <div class="thumb-new-container">
        <div>
            <img src={news.image} alt={news.title}/>
        </div>
        <div class="news-content">
            <div>
                <h1>{news.id}</h1>
                <h2>{news.title}</h2>
                <p>{news.description}</p>
            </div>
        </div>
    </div>
{/each}