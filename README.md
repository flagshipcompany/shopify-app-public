# FlagShip for Shopify App

- [About the FlagShip for Shopify App](#about-the-flagship-for-shopify-app)
- [Features](#features)
- [Considerations](#considerations)
- [Getting Started With the FlagShip for Shopify app](#getting-started-with-the-flagship-for-shopify-app)
- [FlagShip for Shopify app settings](#flagship-for-shopify-app-settings)
- [Pending Orders](#pending-orders)
- [Prepared Orders](#prepared-orders)
- [Schedule Pickups](#schedule-pickups)
- [Pickup Form](#pickup-form)
- [View Pickups](#view-pickups)
- [Product Features](#product-features)
- [View Products](#view-products)
- [View/Create Boxes](#view-boxes)
- [Report Issues](https://github.com/flagshipcompany/shopify-issues/issues)

##About the FlagShip for Shopify App
FlagShip™ for Shopify is bringing reliable discounted shipping to your online store faster, easier and more affordably.  Instantly upload data, print labels, process shipments, share real-time rates or set shipping rates on your online store - and more!  Manage shipments for online purchases easily and take your Shopify store to the next level with FlagShip.

##Features
* Get real-time discounted shipping rates from FlagShip's online shipping system to your Shopify store.
* Print your labels from the app.
* Manage pickups from the app.
* Push any order to FlagShip's online shipping system to create a prequoted shipment (useful if you don't have realtime quoting available in your Shopify Plan).
* Easy way of adding residential surcharges to the quoted price.

##Considerations
 * Only "Unlimited" Shopify plans will benefit from real time quoting. Shops with a lesser plan will still be able to offer standard and/or flat rate shipping to their online store and send shipment information to FlagShip's online shipping system through the FlagShip for Shopify App.
 * Since Shopify does not provide dimensions of your store goods, the shipping rate is made by weight only. Make sure you enter the dimensional weight for your goods if necessary for large but light items.

## Connecting the app to the FlagShip API

When the app is installed, you will be taken to this page where you register your token to the app.

![Token Register Page](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/token_register.png)


### Create Token Credentials
Go to https://auth.smartship.io, **login with your FlagShip credentials** and create a set of credentials using the Shopify Preset

*NOTE: Only FlagShip Account Managers can access the credentials page*

![Auth Page](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/auth.png)

**copy** or keep this page open, as we will need some information from this `token` that was created.

### Register your access token

Insert the **Active token** text from the token that we just created into the **Access token** field.

![inputs](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/token_key_inputs.png)

Submit the keys by pressing the **Save token credentials** button. If the key pair is valid, you will have successfully linked your app to the FlagShip API.

You now have full access to the FlagShip for Shopify app.

If for any reason, your token gets deleted, you will be redirected to this page if you ever access the app, as your token does not exist and is not considered valid. You will need to create a new token if you wish to continue using the app.

## Getting Started With the FlagShip for Shopify app
Here are the menu options that can be done in the app

![Main Menu](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/main_menu.png)

* **Pending Orders**
Allows you to complete orders using FlagShip's online shipping system and dispatch them.
* **Prepared Orders**
Allows you to view dispatched shipments, request documents and view the shipment overview (done on the FlagShip online shipping system).
* **Pickups**
Allows you to schedule pickups for dispatched shipments, view pickups and cancel scheduled pickups.
* **Products**
Allows you to save your product's dimensions, as well as create boxes that will be used when generating rates and dispatching orders on the FlagShip API
* **Settings**
Change app settings that modify quoting and shipment options when dispatching using FlagShip's online shipping system.

### FlagShip for Shopify App Settings

* **Services**
Checkboxes consisting of the courier services that FlagShip offers, and a list of the various services types that the couriers will offer. You can use these checkboxes to show or hide certain couriers or services so that they will not appear in the *shipping method* menu at checkout.

* **Packaging**
Allows you to set the unit of measurement you wish to use when setting your products and box dimensions, and the unit of measurement used when generating rates, dispatching, and prequoting orders on the app.

* **Additional Charges**
Allows you to add a residential surcharge during the quoting process and dispatch process. This helps get more accurate rates during the quoting process and the dispatch process. You can also choose to insure orders that are made through your store with FlagShip's discounted insurance program.

### Pending Orders

This is the page where you can see all the orders that have been placed by customers. 

![Pending Orders](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/pending_orders.png)
This page also allows you to take orders and convert them to a shipment using the FlagShip online shipping system. You can also automatically dispatch orders from this page as well, provided the order was quoted with a FlagShip service.

Upon installing the app, it will fetch all the orders your store has not marked as shipped from the past thirty days and add them to the app's records so that you can start using the FlagShip for Shopify app right away.

* **Order Number**
The order number as it appears in your Shopify admin store. Links to the overview for the order in your Shopify admin page.

* **Order Date**
The date the order was placed on.

* **Courier Used**
The courier used or the company who provides the shipping service (ex: UPS, FedEx, Purolator, etc.).

* **Service Used**
The shipping service selected by the customer.

* **Quoted Price**
The price that was displayed to the customer at the shipping method page in your storefront.

* **Is Fufilled**
Checks to see if the order has been fufilled in your admin page. An order is considered fufilled by the app when you mark the order as having been fully paid in your Shopify admin page.

#### Actions
An action that can be taken for the order, usually in the form of a button or a link. Different factors will determine what will be shown and what actions it will take.
  
* **Convert order on FlagShip**
![Convert Order](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/convert_order.png)
Any online store order that was processed via the FlagShip for Shopify App using a standard or flat rate must be sent to the FlagShip online shipping system to select your choice of service, courier rate and to complete your shipment. 
**Note**: you will not be charged for completing this action on the FlagShip for Shopify App. However, when you complete your order and dispatch it through the FlagShip online shipping system, you will be charged for this order.

* **Dispatch Order to FlagShip**
![Dispatch Order](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/dispatch_order.png)
Any online store order that was processed via the FlagShip for Shopify App using live courier rates can be immediately dispatched to the FlagShip online shipping system by pressing the **Dispatch Order to FlagShip** button. This will automatically create the necessary documents you need to send the shipment to your customer, such as the shipping labels and the commercial invoices, if necessary. If your order has been fulfilled in your store's admin page, a prompt will appear asking you to confirm the dispatch. This extra step is for your benefit and ensures you do not dispatch an order that has already been sent out **or** so you do not get charged for an order that you do not plan on shipping.
**Note**: By dispatching an order using the FlagShip for Shopify App, you will be charged for the dispatched order on the FlagShip online shipping system.

* **View on FlagShip**
![View On FlagShip](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/view_on_flagship.png)
Allows you to either see the overview for your order or continue the quoting process on the FlagShip online shipping system. If your order was prequoted using the app, the link will bring you to the quote page for your order on the FlagShip online shipping system. If the order was dispatched using the app, then the link will be the same, but will instead take you to the shipment overview page for the order on the FlagShip online shipping system.

### Prepared Orders
This allows you to see all the orders you have dispatched using the FlagShip for Shopify app and online system.
![Shipments Page](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/shipments.png)

* **Order Number**
The order number as it appears in your Shopify admin store. Links to the overview for the order in your Shopify admin page.

* **Tracking Number**
The tracking number for the order.

* **To Address**
The destination of the order, as well as its intended receiver, either a company name or the name of a person.

* **Service Used**
The service that was used when the order was dispatched. 

* **Total Cost**
The total cost that was quoted when the order was dispatched.

* **Shipping Documents**
![Shipment Options](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/shipment_documents.png)
The list of shipping documents that are required when dispatching your order to the couriers. Every dispatched shipment will link to a regular sized label and a thermal label. A label must be placed on each of the packages in your shipment. For international shipments, there is a commercial invoice document that must also be included in the shipment along with the shipping labels. All the documents are in .PDF format. Note that shipments that have not been dispatched or that have been cancelled will have no shipping documents available.

* **Cancel Order**
![Cancel Button](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/cancel_shipment.png)
Allows you cancel the order that was made using the FlagShip online shipping system. Note that cancelling an order that was made **will not** cancel any pickups made for that order automatically. They must be cancelled manually using the app. Orders that have been cancelled will have their rows highlighted in red.

* **View On FlagShip**
Allows you to either see the overview for your order or continue the quoting process on the FlagShip online shipping system. If your order was prequoted using the app, the link will bring you to the quote page for your order on the FlagShip online shipping system. If the order was dispatched using the app or by other means, then the link will be the same, but will instead take you to the shipment overview page for the order on the FlagShip online shipping system.

###Pickups
This link will bring you to the pickup actions page. From here, you can navigate to the **Schedule Pickups** page, or the **View Pickups** page.
![Pickup Admin](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/pickup_admin.png)


####Schedule Pickups
From this page, you can schedule pickups for the shipments made through the FlagShip for Shopify app.
![Pending Pickups](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/pending_pickups.png)

* **Tracking Number**
The tracking number for the order.

* **Intended Destination Address**
The destination of the order, as well as its intended receiver, either a company name or the name of a person.

* **Courier**
The courier company which was used in the dispatch.

* **Shipment Date**
The date on which the shipment was made.

* **Check To Schedule**
Checkboxes for which you want to schedule pickups for. You can schedule a single pickup for multiple shipments, provided they are all from the same courier. If the couriers are all the same for the selected shipments, you can then proceed to the schedule pickup page by pressing the **Schedule pickups** button on the bottom right of the page.

####Pickup Form
This is where you fill in the information for your pickup. All of the fields are required to schedule your pickup.
![Pickup Form](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/pickup_form.png)

* **Pickup address**
This is the address that will be used for the pickup address. This is your store's address information.

* **Pickup Date**
The date when you want to schedule the pickup. Note that all the couriers have different lengths for which you can schedule your pickups ahead of time. In most case, scheduling pickups more than a week ahead of time may result in the request failing.

* **Pickup Location**
A drop down list of pickup locations that are considered valid options by the courier.

* **Delivery Instructions**
Special instructions to the driver for how to handle your shipment or other relevant information.


Once all the information has been filled in, you can proceed by pressing the **Schedule** button. Once that has been done and no errors occur, your pickup is created and you can now view it from the **View Pickups** page.

####View Pickups
This is where you can view all the pickups you have made through the FlagShip for Shopify app. You can also cancel pickups you have already made.

![View pickups](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/view_pickups.png)

* **Confirmation number**
The pickup confirmation number.

* **Pickup Date**
The date when the pickup was made for.

* **Pickup Location**
The location that was provided when the pickup was scheduled.

The next row can have a button that allows you to cancel the pickup, provided that either the shipment has not been picked up by the courier yet, or that the pickup date has not been passed.

Cancelled pickups will have the row highlighted in red and the cancel button is removed.

####Product Features
**New Features**
The View products and View Boxes section of the FlagShip for Shopify app allow you to enter in extra information regarding your products dimensions. It will also allow you to enter and save the boxes that you use when you ship your orders.
![View products](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/products_menu.png)

The two features combined allows the FlagShip API to generate a optimal packaging solution for your orders, which will automatically be used when generating rates at checkout, and dispatching or prequoting orders.

**Note**
**The FlagShip for Shopify app will not calculate rates, dispatch, or prequote orders if you have not entered in the dimensional information for all your products and/or entered correct box sizes.**
You will be notified of the packing errors when you attempt to dispatch or prequote an order if its missing product dimensions or missing boxes. You will also be notified if the FlagShip API could not find a packing solution in these three conditions:

![Box Error](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/packing_error_boxes.png)

This error above means that there are no boxes saved in the FlagShip for Shopify app. You must go to the View/Create boxes page and save a box on the app.

![Product Error](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/product_error_product.png)

The error shown above means that the product mentioned in the error message is missing dimensions. You must go to the Product List page and enter in the dimensions for the product in question. This error message will appear once for each product that is missing dimensions within an order, so this message can appear multiple times in the same order.

![Packing Error](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/packing_error.png)

The error shown above means that based on the given products in the order, and the boxes saved in the app, the FlagShip API cannot provide a packing solution for this order. This is usually caused because one of the products in the order cannot fit inside any or the boxes provided in a normal fashion. To resolve this issue, it is recommended that you have a box that can fit the products you have listed in your store.

####View Products
From this page, you can enter in the dimensions of each of your store's products.

![View products](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/product_list.png)

For each product you have in your store, you can enter in their dimensions using the unit of measurement shown in the message under the title, with either centimeters (cm), or inches (in) being the supported dimensions.

####View Boxes
This page allows you to create, edit, and delete boxes that your Shopify store uses when shipping orders.

![View products](https://raw.githubusercontent.com/flagshipcompany/shopify-app-public/master/img/box_list.png)

To create a new box, simply press the **Add New Box** button and a new row will appear where you can fill out your box's dimensions, a maximum weight that your box can support, the weight of the box when empty, and a name for the box being entered.

