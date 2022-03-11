<script>
    export let type = "default";

</script>

<p class="{type}"> <slot/></p>

<style>

p {
padding-left:  0.6rem;
padding-right:  0.6rem;
padding-top:  0.2rem;
padding-bottom:  0.2rem;
width: fit-content;
border-radius: 12px;
color: var(--primary-font-color);
background: var(--default-color);
 font-family: var(--font-family);
 font-weight: 500;
}

.primary {
background-color: var(--primary-color);
    }


.secondary {
background-color: var(--secondary-color);
    }


.accent {
background-color: var(--accent-color);
}

.ghost {
 background-color: var(--ghost-color);
 color: var(--ghost-color);
     
}



</style>