<script>
import Button from "./Button.svelte";
import Badge from "./Badge.svelte"

  export let number;
  export let buttonbadgetext;
</script>

<div class="container">
    <div class="badge">
    <Badge type="secondary">
        <p class="text">{number}</p>
    </Badge>
    </div>
      <div class="button">
    <Button>{buttonbadgetext}</Button>
</div>
</div>


<style>

.container {

    position: relative;
}
  
  .badge {
    position:absolute;
    z-index: 1;
    left: 50px;
    bottom: 24px;
  
     
  }

  p {
font-size: 0.8rem;


  }
</style>