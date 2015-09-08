# Smartship Shopify App (BETA)

- [Features](#features)
- [Installation](#installation) 
- Settings
- [Report Issues](https://github.com/flagshipcompany/shopify-issues/issues)

##Features
* Get realtime discounted rates from Smartship with your Smartship Account
* Automatically complete a shipment when the funds are captured
* Print your labels from the app
* Manage pickups from the app
* Split the shipment in several boxes depending on weight
* Push any order to Smartship to create a prequoted shipment (useful if you don't have realtime quoting available in your Shopify Plan)
* Easy way of adding residential surcharges to the quoted price

##Installation
### Create Credentials
Go to https://auth.smartship.io and create a set of credentials using the Shopify Preset
*NOTE: Only Account Manager can access the credentials page*

![Auth Page](/img/auth.png)

**copy** the new `key`, we will use it later in the Shopify App to connect your Smartship Account with Shopify.

### Install the App
#### BETA installation

You need to create copy paste this link in your browser, while replacing the name of your shop:

`https://shopify.smartship.io/remote-install?shop=MY_SHOP_NAME.myshopify.com`

You need to replace `MY_SHOP_NAME` with the actual name of your shop, e.g 
if the name of your shop is `awesomecandies.myshopify.com` you need to go to this address:
`https://shopify.smartship.io/remote-install?shop=awesomecandies.myshopify.com`

*NOTE: One we're out of beta, the app will be available in the Shopify App Store*

Accept the permissions it needs and you're almost done! 

#### Connecting the App to Smartship
Go into Settings and at the bottom it will ask for your smartship key. This is the one we created earlier in this help file.
Save it by clicking the top right corner button and you're ready to show real time rates! (with the appropriate Shopify Plan)
