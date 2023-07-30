<template>
    <nav class="navigation">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/tunes">Tunes</RouterLink>
        <RouterLink to="/about">About</RouterLink>
    </nav>
</template>

<style lang="scss" scoped>
nav {
	margin: 2em auto 2.5em;
	padding: 0 1.25em;
	display: inline-block;

	vertical-align: middle;
	background: transparent;
	white-space: nowrap;

	border: 3px solid white;
	border-radius: 2.5em;

	a {
		color: white;
		font-size: 1.1em;
		font-weight: 800;
		text-decoration: none;

		cursor: pointer;
		padding: 0.575em 0.65em;
		display: inline-block;

		&.router-link-exact-active {
			color: #fffa0d;
		}
	}
}
</style>