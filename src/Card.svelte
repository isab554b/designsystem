<script>
import Button from "./Button.svelte";
import Badge from "./Badge.svelte"
</script>


<div class="card-component">
<img src="/shoes.jpg" alt="sko">
<div class="h3-badge">
 <h3>Shoes!</h3>
 <Badge type="secondary">NEW</Badge>
 </div>
 <div class="description">
 <p>If a dog chews shoes whose shoes does he choose?</p>
 </div>
 <div class="category-container">
 <p class="category">Fashion</p>
 <p class="category">Products</p>
 </div>
 <div class="buy-now">
 <Button type="primary" >BUY NOW</Button>
 </div>
</div>

<style>
    img {
        width:300px;
        height: 180px;
       object-fit: cover; 
       border-radius: 12px 12px 0 0;
       object-position: 20% 60%;
    }

    .card-component {
        border-radius: 12px;
        width: fit-content;
        font-family: var(--font-family);
        background-color: var(--primary-font-color);
        
    }

    .h3-badge {
        display: flex;
        flex-direction: row;
        gap: 1rem;
        margin-top: -0.5rem;
        margin-left: 1rem;
    
    }

    .description {
        font-size: 0.7rem;
        margin-top: -1rem;
        margin-right: 1rem;
        margin-left: 1rem;
    }
 
    .category-container {
        display: flex;
        flex-direction: row;
        gap: 0.5rem;
        margin-top: -1rem;
        margin-left: 1rem;
        font-size: 0.75rem;
    }

    .buy-now {
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        padding-right: 1rem;
        padding-bottom: 1rem;

    }

    .category {
        border: 1px solid black;
        border-radius: 12px;
        padding: 0 0.5rem 0 0.5rem;
  }
</style>