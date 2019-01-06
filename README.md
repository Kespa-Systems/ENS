# ENS
## API PHP version 1.0  
  
API for the creation of a signature for shipment and validation in Cartouche.
>

As a first requirement, it must be specified that you are using __PHP 7.2__ and that you have installed the __“gmp”__ module for php in a recent version.

### __Instructions for using the API:__

1. Unzip folder where you want to work the API.

2. By default the system connects with the test credentials to https://api-test.cartouche.co/v2/. To make the change to https://api.cartouche.co/v2/ in the associate.php file, uncomment line 13 and comment on line 12.

3. To test please verify your credentials whether test or production in the file test.private.json (please do not change the name to the file test.private.json)

4. In console, execute the command:
	
	```
	$ php associate.php domain.extension
	```
>

__Optional:__

- You can send the Address as an optional parameter, keep in mind that this prevails over the one written in the file test.private.json.

	`$ php associate.php domain.extension address`

>

If the response of the request is correct, it returns OK otherwise it will show a message with the error.

At this moment you can try the domain enstest.luxe and return ok.
