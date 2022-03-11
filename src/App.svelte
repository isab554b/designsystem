<script>
import Button from "./Button.svelte";
import Badge from "./Badge.svelte"
import Footer from "./Footer.svelte"
import Card from "./Card.svelte"
import ButtonBadge from "./ButtonBadge.svelte"
import Avatar from "./Avatar.svelte"
</script>

<main>
<h2 class="h2-footer">Footer component</h2>
<section class="footer">
<Footer/>
<pre><code>{'<Footer/>'}</code></pre>
</section>

<h2 class="h2-badge">Badge components</h2>
<section class="badge" >
<div class="div-badge">
<h3>Neutral badge</h3>
<Badge>neutral</Badge>
<pre><code>{'<Badge>neutral</Badge>'}</code></pre>
</div>

<div class="div-badge">
<h3>Primary badge</h3>
<Badge type="primary">primary</Badge>
<pre><code>{'<Badge type="primary">primary</Badge>'}</code></pre>
</div>

<div class="div-badge">
<h3>Secondary badge</h3>
<Badge type="secondary">secondary</Badge>
<pre><code>{'<Badge type="secondary">secondary</Badge>'}</code></pre>
</div>

<div class="div-badge">
<h3>Accent badge</h3>
<Badge type="accent">accent</Badge>
<pre><code>{'<Badge type="accent">accent</Badge>'}</code></pre>
</div>

<div class="div-badge">
<h3>Ghost badge</h3>
<Badge type="ghost">ghost</Badge>
<pre><code>{'<Badge type="ghost">ghost</Badge>'}</code></pre>
</div>
	
</section>

<h2 class="h2-button">Button components</h2>
<section class="button" >
<div class="div-button">
<h3>Button</h3>
<Button>BUTTON</Button>
<pre><code>{'<Button>BUTTON</Button>'}</code></pre>
</div>
<div class="div-button">
<h3>Primary button</h3>
<Button type="primary">PRIMARY</Button>
<pre><code>{'<Button type="primary">PRIMARY</Button>'}</code></pre>
</div>

<!-- <Button type="primary" mode="inversed">PRIMARY</Button> -->
<div class="div-button">
<h3>Secondary button</h3>
<Button type="secondary">SECONDARY</Button>
<pre><code>{'<Button type="secondary">SECONDARY</Button>'}</code></pre>
</div>
<!-- <Button type="secondary" mode="inversed">SECONDARY</Button> -->

<div class="div-button">
<h3>Accent button</h3>
<Button type="accent">ACCENT</Button>
<pre><code>{'<Button type="accent">ACCENT</Button>'}</code></pre>
</div>

<div class="div-button">
<h3>Ghost button</h3>
<Button type="ghost">GHOST</Button>
<pre><code>{'<Button type="ghost">GHOST</Button>'}</code></pre>
</div>

<div class="div-button">
<h3>Link</h3>
<Button type="link">LINK</Button>
<pre><code>{'<Button type="link">LINK</Button>'}</code></pre>
</div>
</section>

<h2 class="h2-card">Card component</h2>
<section class="card">
<Card img="./shoes.jpg" title="Shoes!" badgetext="NEW" description="If a dog chews shoes whose shoes does he choose?" category1="Fashion" category2="Products" buttontext="BUY NOW" ></Card>

<pre><code>{'<Card img="./shoes.jpg" title="Shoes!" badgetext="NEW" description="If a dog chews shoes whose shoes does he choose?" category1="Fashion" category2="Products" buttontext="BUY NOW"></Card>'}</code></pre>

</section>

<h2 class="h2-buttonbadge">Button w Badge component</h2>
<section class="button-badge">
<ButtonBadge buttonbadgetext="INBOX" number="99+" ></ButtonBadge>
<pre><code>{'<ButtonBadge buttonbadgetext="INBOX" number="99+" ></ButtonBadge>'}</code></pre>	
</section>

<h2 class="h2-avatar">Avatar w indicator</h2>
<section class="avatar" >
<div class="xl">
<h3>XL avatar</h3>
<Avatar size="xl" text="K"></Avatar>
<pre><code>{'<Avatar size="xl" text="K"></Avatar>'}</code></pre>
</div>

<div class="lg">
<h3>LG avatar</h3>
<Avatar size="lg" text="JO"></Avatar>
<pre><code>{'<Avatar size="lg" text="JO"></Avatar>'}</code></pre>
</div>

<div class="md">
<h3>MD avatar</h3>
<Avatar size="md" text="MX"></Avatar>
<pre><code>{'<Avatar size="md" text="MX"></Avatar>'}</code></pre>
</div>

<div class="sm">
<h3>SM avatar</h3>
<Avatar size="sm" text="AA"></Avatar>
<pre><code>{'<Avatar size="sm" text="AA"></Avatar>'}</code></pre>
</div>

</section>
</main>



<style>

.xl {
	background-color: var(--primary-font-color);
	padding: 0.5rem 0 1rem 1rem;
	border-radius: 12px;
}

.lg {
	background-color: var(--primary-font-color);
	padding: 0.5rem 0 1rem 1rem;
	border-radius: 12px;
}

.md {
	background-color: var(--primary-font-color);
	padding: 0.5rem 0 1rem 1rem;
	border-radius: 12px;
}

.sm {
	background-color: var(--primary-font-color);
	padding: 0.5rem 0 1rem 1rem;
	border-radius: 12px;
}

section {
	margin-bottom: 4rem;
}

.h2-footer {
	padding-left: 2rem;	
}
.h2-buttonbadge {
padding-left: 2rem;	
}
.h2-badge {
	padding-left: 2rem;
}
.h2-button {
	padding-left: 2rem;
}
.h2-avatar {
	padding-left: 2rem;
}

.h2-card {
	padding-left: 2rem;
}


.badge {
	display: grid;
	    grid-template-columns: repeat( auto-fit, minmax(300px, 1fr) );
		padding: 0 2rem 0 2rem;
		gap: 4rem;
}

.card {
	display: flex;
	flex-direction: column;
	padding: 0 2rem 0 2rem;
	
}



.button-badge {
	padding: 0 2rem 0 2rem;
}

.button {
	display: grid;
	    grid-template-columns: repeat( auto-fit, minmax(300px, 1fr) );
		padding: 0 2rem 0 2rem;
		gap: 4rem;

}

h2 {
	font-family: var(--font-family);
	font-size: 1.2rem;
	
}

h3 {
	font-family: var(--font-family);
font-size: 1rem;
}

.avatar {
	display: grid;
	grid-template-columns: repeat( auto-fit, minmax(200px, 1fr) );
	padding: 0 2rem 0 2rem;
	gap: 4rem;
	font-family: var(--font-family);
	
}

.footer {
	padding: 0 2rem 0 2rem;
}



code {
	font-family: var(--font-family);
	font-size: 0.9rem;
	font-weight: 400;
	padding: 0.2rem;
	border-radius: 12px;
}

.div-button {
	background-color: var(--primary-font-color);
	padding: 0.5rem 0 1rem 1rem;
	border-radius: 12px;
}
.div-badge {
	background-color: var(--primary-font-color);
	padding: 0.5rem 0 1rem 1rem;
	border-radius: 12px;
}

</style>