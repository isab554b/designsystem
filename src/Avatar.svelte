
<script>
    export let size;
export let text;
 
</script>

<div class="{size}">
<p class="text">{text}</p></div>



<style> 

p {

	color: var(--primary-font-color);
}


.xl {
    width: 75px;
    height: 75px;
    background-color: var(--default-color);
    border-radius: 50%; 
}

.lg {
    width: 55px;
    height: 55px;
    background-color: var(--default-color);
    border-radius: 50%; 
}

.md {
    width: 40px;
    height: 40px;
    background-color: var(--default-color);
    border-radius: 50%; 
}

.sm {
    width: 30px;
    height: 30px;
    background-color: var(--default-color);
    border-radius: 50%; 
}

.text {
    position: absolute;

}

</style>

