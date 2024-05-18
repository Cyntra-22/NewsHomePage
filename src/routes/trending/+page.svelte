<script script lang="ts">
    import NavNew from "$lib/NavNew.svelte"; 
</script>
<style> 
    .trending-container {
        display: flex;
        justify-content: space-between;
        margin-bottom: 40px;
        padding-bottom: 20px;
        border-bottom: 1px solid black;
    }
    
    .img-container {
        padding: 10px;
        transition: transform 0.3s ease; 
    }
    
    img {
        width: 225px;
        height: 450px;
        cursor: pointer;
    }
    
    a {
        text-decoration: none;
        color: black;
        cursor: pointer;
    }
    
    .img-container:hover {
        transform: scale(1.05); 
    }
    .new-container{
        display: flex;
        justify-content: space-between;
    }

    @media (min-width: 300px) and (max-width: 768px ){
        .trending-container{
            display:block;
        }
        img{
            width: 100%;
        }
        .new-container{
            display: block;
        }

    }
    
</style>

<div class="trending-container">
    <div class="img-container">
        <img src="/image-retro-pcs.jpg" alt="new title"/>
        <a href="/"><h3>Reviving Retro PCs</h3></a>
    </div>
     <div class="img-container">
        <img src="/image-gaming-growth.jpg" alt="new title"/>
        <a href="/"><h3>Reviving Retro PCs</h3></a>
    </div>
     <div class="img-container">
        <img src="/image-retro-pcs.jpg" alt="new title"/>
        <a href="/"><h3>Reviving Retro PCs</h3></a>
    </div>
     <div class="img-container">
        <img src="/image-gaming-growth.jpg" alt="new title"/>
        <a href="/"><h3>Reviving Retro PCs</h3></a>
    </div>
     <div class="img-container">
        <img src="/image-retro-pcs.jpg" alt="new title"/>
        <a href="/"><h3>Reviving Retro PCs</h3></a>
    </div> 
   
</div>
 <div class="new-container ">
        <NavNew/>
        <NavNew/>
        <NavNew/>
</div>
<div class="new-container ">
        <NavNew/>
        <NavNew/>
        <NavNew/>
</div>

