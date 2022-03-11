<script>
import Button from "./Button.svelte";
import Badge from "./Badge.svelte"

  export let number;
</script>

<div class="container">
    <div class="badge">
    <Badge type="secondary">
        <p class="text">{number}</p>
    </Badge>
    </div>
      <div class="button">
    <Button>INBOX</Button>
</div>
</div>


<style>

.container {
    position: relative;
}
  
  .badge {
    position:absolute;
    z-index: 1;
    top: 0;
  
     
  }
</style>