<script>
    export let type = "default";
    export let mode;
</script>

<button class:inversed={mode==="inversed"} class="{type}"> <slot/></button>

<style>

button {
border: none;
border-radius: 10px;
color: var(--primary-font-color);
background: var(--default-color);
padding: 1rem;
transition: all 0.5s;
cursor: pointer;
font-family: var(--font-family);
font-weight: 600;
}

.primary {
background-color: var(--primary-color);
    }


.primary:hover {
color: var(--primary-color);
background: var(--primary-font-color);
}

/* .primary.inversed {
color: var(--primary-color) ;
background: var(--primary-font-color);

}

.primary.inversed:hover {
color: var(--primary-font-color) ;
background: var(--primary-color);

} */

.secondary {
background-color: var(--secondary-color);
    }


.secondary:hover {
color: var(--secondary-color);
background: var(--primary-font-color);
}


/* .secondary.inversed {
color: var(--secondary-color) ;
background: var(--primary-font-color);

}

.secondary.inversed:hover {
color:  var(--primary-font-color);
background: var(--secondary-color);

} */

.accent {
background-color: var(--accent-color);
}

.accent:hover {
color: var(--accent-color) ;
background-color: var(--primary-font-color);
}

.ghost {
 background-color: var(--ghost-color);
 color: var(--ghost-color);
     
}

.link {
 background-color: var(--link-color);
 color: var(--link-font-color);
     
}

</style>