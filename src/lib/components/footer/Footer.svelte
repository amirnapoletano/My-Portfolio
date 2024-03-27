<script>
	import LogoComponent from '$lib/components/header/LogoComponent.svelte';
	let currentYear = new Date().getFullYear();
</script>

<footer class="footer">
	<h1>
		contact
	</h1>
	<LogoComponent/>
	<p>&#169; {currentYear} New Horizons</p>
	<div>
		<a href="#">Home</a>
		<a href="#">About</a>
		<a href="#">Contact</a>
	</div>
</footer>
<style>
    /* Footer styles */
    .footer {
        background-color: #333;
        color: #fff;
        padding: 20px 0;
        text-align: center;
        position: absolute;
        bottom: 0;
        width: 100%;
    }

    .footer a {
        color: #fff;
        text-decoration: none;
        margin: 0 10px;
    }
</style>

