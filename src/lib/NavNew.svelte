<style>
    img{
        width: 100%;
        height: auto;
        max-height: 200px; 
        object-fit: cover;
        
    }
    .container{
        margin-bottom: 20px;
        
    }

    .content-container{
        width: 98%;
    }

   
    button{
        background-color: var(--button-color);
        color: white;
        padding: 10px 25px 10px 25px;
        border: none;
        cursor: pointer;
        font-size: 15px;
        font-weight: bold;
        
    }

    button:hover{
        color: white;
        background-color: black;
        
    }

    p{
        text-align: justify;
       
    }
   

     @media (min-width: 300px) and (max-width: 768px ){
        .container{
            width: 100%;
        }
        img{
            width: 100%;
        }
    }
    
</style>

<div class="container">
    <div class="content-container">
        <img src="/image-top-laptops.jpg" alt="new title"/>
        <h1>Rebuilding the pipeline for local news</h1>
        <p>We work toward this goal every day with emerging journalists through our Report for America program, but the urgency of this moment means we need to widen the circle.</p>
        <button>See More</button>
    </div>
</div>