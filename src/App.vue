<template>
	<div id="app">
		<header class="header">
		  <strong>
		    <g-link to="/">{{ $static.metaData.siteName }}</g-link>
		  </strong>

		  <nav class="nav">
		    <g-link class="nav__link" to="/">Home</g-link>
		    <g-link class="nav__link" to="/about">About</g-link>
		  </nav>

		</header>

		<main>
			<g-view />
		</main>

		<footer>
			Copyright {{ $static.metaData.siteName }} 2020
		</footer>
	</div>
</template>

<script>
export default {
	props: ['transparent']
}
</script>
