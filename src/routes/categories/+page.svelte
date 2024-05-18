<script lang="ts">
    import Category from "$lib/Category.svelte";
</script>
<style>
    .list-container{
        display: flex;
        justify-content: space-between;
        padding-bottom: 35px;
        border-bottom: 1px solid var(--text-color);
    }
    a{
        text-decoration: none;
        color: black;
    }
    li{
        list-style-type: none;
        
    }
    h1{
        margin-bottom: 40px;
        text-align: center;
        background-color: var(--button-color);
        padding: 15px;
        letter-spacing: 4px;
        color: white;
    }

    a:hover{
        color: var(--button-color);
    }
    .item-display{
        display: flex;
    }

    @media (min-width: 300px) and (max-width: 768px ){
        .item-display{
            display: block;
        }
         .list-container{
            display: block;
         }
         li{
            list-style-type:square;
            
         }
    }

</style>

<div>
    <h1>CATEGORIES</h1>
    <div class="list-container">
        <li><a href="#content-policy">Content Policy</a></li> 
        <li><a href="#freedom-of-expression">Freedom of Expression</a></li> 
        <li><a href="#human-right">Human Right</a></li> 
        <li><a href="#legal-and-regulatory">Legal and Regulatory</a></li> 
        <li><a href="#socioculture">Socioculture</a></li> 
        <li><a href="#laws-business">Laws and Business</a></li> 
    </div>
    <div>
        <h2>Related News</h2>
        <Category/><hr/>
        <Category/><hr/>
        <Category/><hr/>
        <Category/><hr/>
    </div>
   
    <div id="content-policy">
        <h2>Content Policy</h2>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
    </div>
    <hr/>
     <div id="freedom-of-expression">
        <h2>Freedom of Expression</h2>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
    </div>
    <hr/>
     <div id="human-right">
        <h2>Human Right</h2>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
    </div>
    <hr/>
     <div id="legal-and-regulatory">
        <h2>Legal and Regulatory</h2>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
    </div>
    <hr/>
     <div id="socioculture">
        <h2>Socioculture</h2>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
    </div>
    <hr/>
    <div id="laws-business">
        <h2>Laws and Business</h2>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
        <div class="item-display">
            <Category/>
            <Category/>
        </div>
    </div>    
</div>