<script lang="ts">
  import type { newitems } from "./data";

    
    import type { Item2 } from "./types";
    export let newitem: Item2;
    
</script>

<style>
    .multple-new-container{
        padding-bottom: 10px;
        
    }
    h3{
        font-size: 22px;
    }

    h3:hover{
        color: var(--title-color);
        cursor: pointer;
        
    }
    p{
        color: hsl(36, 100%, 99%);
        opacity: 0.7;
    }
</style>

<div class="multple-new-container">
    <h3>{newitem.newTitle}</h3>
    <p>{newitem.newDescription}</p>
</div>