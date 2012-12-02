Overview:
--------
Provides two catalog display types that allow buying multiple items with one click. The catalog display types look the same as the default list table and grid formats, but without the add to cart buttons for individual products and with a button at the bottom of the catalog page instead. When the button is pressed all products with positive quantity field values will be added to the cart.
There are several things to note:

    * This module requires patch at http://www.ubercart.org/issue/4936/a_hook_catalog_renderers to work.
    * It adds a quantity field for each product (just in the multi-buy catalog pages) regardless of whether it's usually a hidden default value).
    * All quantity fields in the multi-buy catalog pages are set to 0 regardless of default quantities set for the products.
    * The multi-buy list table and multi-buy grid formats use all the corresponding settings for the default list table and grid formats.
    * It works with attributes (uc_extra_column for table list).
    * Attribute option select fields that are required are set to their default option rather than the normal "Please select" option. This is so that standard Drupal form validation doesn't balk when an option isn't selected on products where the quantity is set to 0 (ie the customer doesn't want to purchase the product but the form validation requires an option be selected for it's required attribute(s)). It's not an elegant solution but there were time constraints... For this reason it's recommended to not have "required" attributes (the user still has to select an option anyway, and in this context it produces more sensible possible form values).
    * It supports uc_donation products.


Requires:
--------
 - Drupal 6.x
 - Ubercart 6.x-2.2


Credits:
-------
 - Author: Oliver Coleman, oliver@e-geek.com.au, e-geek.com.au, enviro-geek.net
 - Work partially funded by Data-Scribe, www.datascribe.biz


