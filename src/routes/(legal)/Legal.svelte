<script lang="ts">
	import { page } from '$app/stores';

	export let pageTitle: string;

	function classWithPathname(pathname: string): string {
		return $page.url.pathname === pathname ? 'active' : '';
	}
</script>

<svelte:head>
	<title>Sandstorm Sandcats: {pageTitle}</title>
	<style>
		body {
			font-family: sans-serif;
			background-color: #eee;
			padding: 0;
			margin: 0;
		}

		section > * {
			margin: 1em auto;
			max-width: 640px;
			box-sizing: border-box;
		}

		h1 {
			font-size: 25pt;
		}

		h3 {
			font-size: inherit;
		}

		#terms,
		#privacy {
			position: absolute;
			background-color: white;
			border-top: 1px solid #888;
			width: 100%;
		}

		nav ul {
			margin: 0px auto;
			margin-block-end: -1px;
			max-width: 640px;
		}

		nav ul li {
			border: 1px solid #888;
			border-bottom: none;
			background-color: white;
			display: inline-block;
			height: 15px;
			margin: 0px 2px;
			padding: 8px 0;
			position: relative;
			text-align: center;
			width: 190px;
		}

		nav ul li:first-child {
			margin-left: -20px;
		}

		li.active {
			z-index: 1;
		}

		@media screen and (max-width: 650px) {
			section > * {
				width: 100%;
				padding-left: 8px;
				padding-right: 8px;
			}
			nav ul {
				margin: 0px 8px;
				margin-block-end: -1px;
				width: 100%;
			}
			nav ul li {
				width: 46%;
			}
		}
	</style>
</svelte:head>

<div class="legal">
	<section id="overview">
		<h1>Overview: Sandstorm Sandcats</h1>

		<p>
			Sandstorm is a platform for server-oriented and web-based applications. Sandstorm the platform
			is open source; anyone can run Sandstorm on their own personal server hardware. When you run
			Sandstorm on your own hardware, you can do anything you want with it: Sandstorm the platform
			is licensed under the Apache 2.0 open source license which places no restrictions on usage.
		</p>

		<p>
			Sandstorm Development Group, Inc., is the company that distributes the Sandstorm software. It
			also offers a DNS service called Sandcats. Sandcats makes it easy to obtain a hostname and TLS
			certificate for your personal Sandstorm server, as a subdomain of sandcats.io. Sandstorm
			Development Group, Inc., owns the domain sandcats.io but delegates a subdomain, such as
			"example.sandcats.io", to you for free. The purpose of the service is to make it easy for you
			and your friends to easily find your Sandstorm server on the network and ensure that they are
			communicating with it securely. Basically, it acts like a phone book. The Sandcats service
			never sees any of the content of your server nor any of the traffic to your server.
		</p>
	</section>
	<nav>
		<ul>
			<li class={classWithPathname('/terms')}>
				<a href="/terms">Terms of Service</a>
			</li>
			<li class={classWithPathname('/privacy')}>
				<a href="/privacy">Privacy Policy</a>
			</li>
		</ul>
	</nav>
	<slot />
</div>
