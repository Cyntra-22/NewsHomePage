<script lang="ts">
    import Category from "$lib/Category.svelte";
    import NavNew from "$lib/NavNew.svelte";
</script>
<style>
    .popular-display{
        display: flex;
        justify-content: space-between;
        margin-bottom: 30px;
    }

    h2{
        color: black;
        border-bottom: 3px solid var(--button-color);
        margin-right: 30px;
        padding-bottom: 8px;
        
    }
    .new-container{
        display: flex;
        justify-content: space-between;
    }

     @media (min-width: 300px) and (max-width: 768px ){
        .new-container{
            display: block;
        }
        .popular-display{
            display: block;
        }

     }
   
</style>
<div class="popular-display">
    <div >
        <h2>Most Popular</h2>
        <Category/>
        <Category/>
        <Category/>
        <Category/>
    </div>
    <div>
        <h2>Editors' picks</h2>
        <Category/>
        <Category/>
        <Category/>
        <Category/>
    </div>
    <div>
        <h2>Top News</h2>
        <Category/>
        <Category/>
        <Category/>
        <Category/>
    </div>
       
</div>
<hr/>
<h1>Related News</h1>
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