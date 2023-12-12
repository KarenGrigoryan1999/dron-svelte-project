<script>
	import { page } from '$app/stores';
	import github from '$lib/images/github.svg';
</script>

<header>
	<nav>
		<ul>
			<p>Хэдер сайта</p>
			<img src={github} alt="GitHub" />
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/my-test-route">Test page</a>
			</li>
		</ul>
	</nav>
</header>

<style>
	header > nav > ul {
		display: flex;
		flex-direction: row;
	}

	header > nav > ul > img {
		width: 50px;
	}

	li {
		margin: 10px;
	}
</style>
