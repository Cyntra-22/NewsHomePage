<script>
    
</script>

<style>
    .nav-container{
        width: 80%;
        margin: 30px auto;
        padding: 10px;
    }
        .header{
        display: flex;
        justify-content: space-between;
    }
       
        ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        overflow: hidden;
        }

        li {
        float: left;
        }

        li a {
        display: block;
        color: black;
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
        cursor: pointer;
        }

        li a:hover {
        color: var(--button-color);
        }
        .show-menu{
            display: none;
        }
        button{
            border: none;
            background-color: transparent;
            cursor: pointer;
            padding-top: 15px;
        }
        

        @media (min-width:300px ) and (max-width: 600px){
           
            .show-menu{
                display: block;
            }
           ul{
            display: none;
           }
        
        }
</style>

<div class="nav-container">  
    <div class="header">
        <div>
            <img src="/logo.svg" alt="logo"/>
        </div>
        <div>
            <button class="show-menu" ><img src="/icon-menu.svg" alt="nav icon"></button>
                <ul >
                    <li><a href="/">Home</a></li>
                    <li><a href="/newnav" >News</a></li>
                    <li><a href="/popular" >Popular</a></li>
                    <li><a href="/trending" >Trending</a></li>
                    <li><a href="/categories" >Categories</a></li>
                </ul>          
        </div>  
    </div>
</div>