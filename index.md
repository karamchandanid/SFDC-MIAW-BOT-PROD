<html lang="en">
  <head>
    <title>
		      MIAW: UAT Demo
		</title>
		<style>
      h1 {
        display: none;
      }
    </style>
		<script>
			window.addEventListener("onEmbeddedMessagingReady", (evt) => {
			    // The JavaScrip API is ready for calls.
			    console.log("Received the onEmbeddedMessagingReady event…");
			    console.log(">>",evt);
			});
		</script>
  	<script type='text/javascript'>
  		function initEmbeddedMessaging() {
  			console.log('initEmbeddedMessaging');
  			try {
  				console.log('initEmbeddedMessaging', 'embeddedservice_bootstrap');
  				embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
  				
  				console.log('initEmbeddedMessaging','embeddedservice_bootstrap','init');
  				embeddedservice_bootstrap.init(
    				'00D600000007Dpt',
    				'Github',
    				'https://legrandav.my.site.com/ESWGithub1722163913919',
    				{
    					scrt2URL: 'https://legrandav.my.salesforce-scrt.com'
    				}
    			);
  				console.log('initEmbeddedMessaging','embeddedservice_bootstrap','done');
  			} catch (err) {
  				console.error('Error loading Embedded Messaging: ', err);
  			}
  		};
  	</script>
  	<script type='text/javascript' src='https://legrandav.my.site.com/ESWGithub1722163913919/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  </head>
  <body >
	  <h2> Hello MIAW-BOT - PRE-Release</h2>
  </body>
</html>
