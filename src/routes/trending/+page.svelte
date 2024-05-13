<script>
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
    }
    
    a {
        text-decoration: none;
        color: black;
    }
    
    .img-container:hover {
        transform: scale(1.05); 
    }
    .new-container{
        display: flex;
        justify-content: space-between;
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

