# Commerce Custom Product

Commerce allows you to sell customizable products that require customer input when added to the cart. Use cases for this functionality include:

* Business cards that require contact information and a logo upload.
* Event registrations that require attendee information.
* Donations the allow the customer to specify a donation amount.

The core Line Item module accommodates these scenarios by letting you add any number of fields to the Product line item type and expose them to the Add to Cart form. However, sites that sell multiple types of customizable products or a mixture of customizable and non-customizable products need to define multiple line item types to handle the different configurations of fields. That's where this Customizable Products module comes in!

It gives you the ability to define new line item types on the fly at **Administration > Store > Configuration > Line item types**. This is functionally equivalent to defining the new line item type in code, which is still recommended if you are able (see below).

## Installation

* Install this module using the [official Backdrop CMS instructions](https://backdropcms.org/guide/modules)

## Configuration

This module only requires the core Line Item and Line Item UI modules to work. Browse to the line item types configuration page and create your new product line item type to begin adding fields to it. Be sure to click the checkbox to include your custom fields on the Add to Cart form or they will not show up.

Once your customizable product line item type has been created, you need to either update an existing product display node type or create a new one to use the custom product line item type. Do this through the settings form for the Add to Cart form display formatter of your node type's Product reference field. If the Add to Cart form is visible on multiple view modes, make sure you have updated them all to use the same line item type.

## Current Maintainers

* Seeking maintainers.

## Credit

Originally maintained on Drupal by:

* https://www.drupal.org/u/rszrama
* https://www.drupal.org/u/centarro

## License

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.
