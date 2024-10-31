<html>
	<body>

      <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">
      
      <script type='text/javascript'>
      	function initEmbeddedMessaging() {
      		try {
      			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

            window.addEventListener("onEmbeddedMessagingReady", e => {
					  embeddedservice_bootstrap.prechatAPI.setVisiblePrechatFields({
					    // List the pre-chat field names with the value and whether
					    // it's editable in the pre-chat form.
					    	"Account_Code": {
					      "value": "AA123",
					      "isEditableByEndUser": true
					    },
	 					"_email": {
					      "value": "tguirgis@testemail.com.invalid",
					      "isEditableByEndUser": true
					    }
	 				  });
					});
            
      			embeddedservice_bootstrap.init(
      				'00DP0000003zzZf',
      				'NAT_Chat_Web',
      				'https://fleetcorna--stagingdev.sandbox.my.site.com/ESWNATChatWeb1730336855134',
      				{
      					scrt2URL: 'https://fleetcorna--stagingdev.sandbox.my.salesforce-scrt.com'
      				}
      			);
      		} catch (err) {
      			console.error('Error loading Embedded Messaging: ', err);
      		}
      	};
      </script>
      <script type='text/javascript' src='https://fleetcorna--stagingdev.sandbox.my.site.com/ESWNATChatWeb1730336855134/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
    </body>
</html>
