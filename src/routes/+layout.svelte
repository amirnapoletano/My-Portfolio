<script>

	// Import Components
	import Header from "$lib/components/header/Header.svelte";
	import Footer from "$lib/components/footer/Footer.svelte";
	// Import Style
	// import './styles.css';

</script>


<div class="app">
	<Header></Header>
	<main class="container">
	<div class="row">
		<slot></slot>
	</div>
	 </main>
<Footer></Footer>
</div>