<footer>
<div>
<h3>SERVICES</h3>
<a href="#">Branding</a>
<a href="#">Design</a>
<a href="#">Marketing</a>
<a href="#">Advertisement</a>
</div>

<div>
<h3>COMPANY</h3>
<a href="#">About us</a>
<a href="#">Contact</a>
<a href="#">Jobs</a>
<a href="#">Press kit</a>
</div>

<div>
<h3>LEGAL</h3>
<a href="#">Term of use</a>
<a href="#">Privacy policy</a>
<a href="#">Cookie policy</a>
</div>
</footer>

<style>

footer {
    color: var(--primary-font-color);
    background-color: var(--default-color) ;
    display: grid;
    grid-template-columns: repeat( auto-fit, minmax(250px, 1fr) );
    padding: 2rem 0 3rem 3rem;
    border-radius: 5px;
    font-family: var(--font-family);
}

div {
display: flex;
flex-direction: column;
gap:0.8rem;
}

a {
color: var(--primary-font-color);
text-decoration: none;
}


h3 {
    opacity: 60%;
}

@media screen and (max-width: 600px) {
  footer {
          grid-template-columns: repeat( auto-fit, minmax(200px, 1fr) );
  }
 
}


</style>