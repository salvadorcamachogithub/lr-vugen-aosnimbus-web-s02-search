Updated: 02.2025
Script created by Salvador Camacho

This script was created with best practices, so it is more resilient, such as:
* Transaction naming
* No add cookies
* No third party
* One validation per transaction
* Think times at the end of each transaction to better simulate user behavior
* Main URL parametrized, Nimbus AOS by default: (http://nimbusserver.aos.com:8000)

This script does a search, then randomly selects a product from the search and then goes to it in transaction number 3 and adds it to the cart to then abandon the cart
The Add To Cart step is "simulated" (it hits a random AOS product image) as there is no http traffic in AOS when adding to the cart
	
Runtime Settings were set to log only on errors and generate snapshot on errors, think times 75% to 150%

This script has 5 transactions
AOS-Web-S02-01 Access AOS URL
AOS-Web-S02-02 Search
AOS-Web-S02-03 Random Product
AOS-Web-S02-04 Add To Cart
AOS-Web-S02-05 Checkout