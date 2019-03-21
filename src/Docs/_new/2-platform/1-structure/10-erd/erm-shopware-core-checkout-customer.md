Customer
---------------------------------------

The central customer entity of the platform. Is created through SalesChannel processes and used in the order and cart workflow.

![Customer](dist/erm-shopware-core-checkout-customer.svg)


### Table `customer`

The main customer table of the system and therefore the entry point into the customer management. All registered customers of any sales channel will be stored here. The customer provides a rich model to manage internal defaults as well as informational data. Guests will also be stored here.


### Table `customer_address`

The customer address table contains all addresses of all customers. Each customer can have multiple addresses for shipping and billing. These can be stored as defaults in `defaultBillingAddressId` and `defaultShippingAddressId` in customer entity itself.


### Table `customer_group`

Customers can be categorized in different groups. The customer group is used so processes like the cart can incorporate different rules.


### Table `customer_group_discount`

Stores a fixed percentage order discount for a specific customer group.

