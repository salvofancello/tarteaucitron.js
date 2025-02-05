


### This is a custom readme for our fork of tarteacitron repository.


# How to use

Include this code in header, edit necessaries options:
- url privacy page;
- add custom scripts if necessary, in this basic versions the scripts present are only for Google Consent mode;

```html
	<script src="/tarteaucitron/tarteaucitron.min.js"></script>
	<script type="text/javascript">
		tarteaucitron.init({
		"privacyUrl": "/privacy", /* Privacy policy url */
		"bodyPosition": "top", /* top to bring it as first element for accessibility */
		"hashtag": "#tarteaucitron", /* Open the panel with this hashtag */
		"cookieName": "tarteaucitron", /* Cookie name */
		"orientation": "bottom", /* Banner position (top - bottom) */
		"groupServices": true, /* Group services by category */
		"showDetailsOnClick": true, /* Click to expand the description */
		"serviceDefaultState": "wait", /* Default state (true - wait - false) */						
		"showAlertSmall": false, /* Show the small banner on bottom right */
		"cookieslist": true, /* Show the cookie list */								
		"closePopup": true, /* Show a close X on the banner */
		"showIcon": false, /* Show cookie icon to manage cookies */
		//"iconSrc": "", /* Optionnal: URL or base64 encoded image */
		"iconPosition": "BottomLeft", /* Position of the cookie (BottomRight - BottomLeft - TopRight - TopLeft) */
		"adblocker": false, /* Show a Warning if an adblocker is detected */
		"DenyAllCta" : true, /* Show the deny all button */
		"AcceptAllCta" : true, /* Show the accept all button */
		"highPrivacy": true, /* HIGHLY RECOMMANDED Disable auto consent */
		"alwaysNeedConsent": false, /* Ask the consent for "Privacy by design" services */								
		"handleBrowserDNTRequest": false, /* If Do Not Track == 1, disallow all */
		"removeCredit": true, /* Remove credit link */
		"moreInfoLink": true, /* Show more info link */
		"useExternalCss": false, /* Expert mode: do not load the tarteaucitron.css file */
		"useExternalJs": false, /* Expert mode: do not load the tarteaucitron js files */
		//"cookieDomain": ".my-multisite-domaine.fr", /* Shared cookie for multisite */									
		"readmoreLink": "", /* Change the default readmore link */
		"mandatory": true, /* Show a message about mandatory cookies */
		"mandatoryCta": false, /* Show the disabled accept button when mandatory on */
		//"customCloserId": "", /* Optional a11y: Custom element ID used to open the panel */
		"googleConsentMode": true, /* Enable Google Consent Mode v2 for Google ads and GA4 */
		"partnersList": true /* Show the number of partners on the popup/middle banner */

		tarteaucitronCustomText = {
			"privacyUrl": "Privacy policy",
		};

		});
			
		(tarteaucitron.job = tarteaucitron.job || []).push('gcmadstorage');
		(tarteaucitron.job = tarteaucitron.job || []).push('gcmanalyticsstorage');
		(tarteaucitron.job = tarteaucitron.job || []).push('gcmpersonalization');
		(tarteaucitron.job = tarteaucitron.job || []).push('gcmfunctionality');
		(tarteaucitron.job = tarteaucitron.job || []).push('gcmadsuserdata');    
		(tarteaucitron.job = tarteaucitron.job || []).push('gcmsecurity');
	</script>
```

# Add a service
[Visit tarteaucitron.io](https://tarteaucitron.io/en/install/)