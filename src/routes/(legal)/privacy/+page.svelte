<script>
	import Legal from '../Legal.svelte';
</script>

<div>
	<Legal pageTitle="Privacy Policy">
		<section id="privacy">
			<h1>Privacy Policy</h1>

			<p>
				This privacy policy describes in detail how the Sandstorm Sandcats DNS service ("the
				service"), as run by Sandstorm Development Group, Inc. ("we"/"us"), protects your privacy.
			</p>

			<p>
				This policy does NOT apply to any other Sandstorm service, such as Sandstorm Oasis. These
				terms also do not apply to users running the Sandstorm open source software under their own
				domain name. Use of the Sandstorm software on your own server (whether under sandcats.io or
				your own domain) is covered by <a
					href="https://github.com/sandstorm-io/sandstorm/blob/master/LICENSE"
					>the Sandstorm license</a
				>.
			</p>

			<h2>Introduction</h2>

			<p>
				The Sandcats service provides DNS (allowing people to locate your computer's IP address
				given the name you choose for it) and TLS certificates (allowing people to establish a
				secure (private and authenticated) connection to your server) to people running a Sandstorm
				server.
			</p>

			<h2>Data gathered from you, and how we use it</h2>

			<p>
				When you run a Sandstorm server that uses Sandcats, the service gathers these pieces of
				information about you:
			</p>

			<ul>
				<li>
					Your server's IP address. This address will be published to the world via the DNS
					protocol, as is the purpose of the service.
				</li>
				<li>
					Your email address. We will use this address to contact you with service issues if needed
					and to help you recover a lost hostname. We will not share this address with anyone unless
					required by law, in which case we will notify you unless prohibited by law.
				</li>
				<li>
					Your chosen Sandcats subdomain. Although we do not actively publish a directory of
					Sandcats hostnames, this name may appear in certificate transparency reports and other
					public places.
				</li>
			</ul>

			<h2>Data gathered by other users' servers</h2>

			<p>
				When you visit a subdomain of sandcats.io, you are visiting someone else's server. This
				server is not controlled by us. You will need to consult that server's own privacy policy to
				determine how it may use your data.
			</p>

			<h2>Data Storage Location</h2>

			<p>
				All data we collect is stored in the United States on servers at our infrastructure service
				provider, Google Cloud Services, which stores this data encrypted at rest. Google Cloud
				Services' <a href="https://cloud.google.com/terms/">Terms of Service</a>, section 5, states
				that Google will use data stored through the service only to deliver the service; data will
				not be used in conjunction with Google's other products, including advertising products.
			</p>

			<h2>Cancellation and data deletion</h2>

			<p>
				You may end your service at any time by stopping your Sandstorm server or reconfiguring it
				not to use Sandcats. If you wish for us to explicitly delete your last-known IP address and
				email address from our database, please contact us at <a href="mailto:support@sandstorm.io"
					>support@sandstorm.io</a
				>.
			</p>

			<h2>Effective Date</h2>

			<p>This policy is effective as of October 6, 2015.</p>
		</section>
	</Legal>
</div>
