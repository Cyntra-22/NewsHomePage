<script lang="ts">
   /* import { onMount } from "svelte";

    let right_image: string = "/image-web-3-desktop.jpg";

    onMount(() => {
        if (window.innerWidth < 1080) {
            right_image = "/image-web-3-mobile.jpg";
        }
    }); */
</script>

<style>
    .flex-container{
        display: flex;
        
    }
    img{
        width: 100%;
    }

    .vertical-center{
        margin-left: 35px;
        padding-top: 20px;
    }
   
    h1{
        font-size: 50px;
        font-weight: 900;
        line-height: 1.1;
    }

    p{
        font-size: 17px;
        color: var(--text-color);
        padding-bottom: 20px;
        line-height: 1.5;
        padding-right: 10px;
    }

    button{
        background-color: var(--button-color);
        color: white;
        padding: 10px 25px 10px 25px;
        border: none;
        cursor: pointer;
        font-size: 15px;
        letter-spacing: 5px;
        font-weight: bold;
    }

    button:hover{
        color: white;
        background-color: black;
        
    }

     @media (min-width: 300px) and (max-width: 768px ){
        .flex-container{
            display: block;
        }
        h1{
            font-size: 40px;
        }
        .vertical-center{
        margin-left: 0px;
        padding-top: 0px;
    }
        p{
            padding-bottom: 10px;
        }
     }

    
</style>

<div>
    <div>
        <img src="/image-web-3-desktop.jpg" alt="new page"/>
        <div class="flex-container">
            <div>
                <h1>The Bright Future of Web 3.0?</h1>
            </div>
            <div class="vertical-center">
                <p>We dive into the next evolution of the web that claims to put the power of the platforms back into the hands of the people. But is it really fulfilling its promise?</p>
                <button>READ MORE</button>
            </div>  
        </div>
    </div>
</div>