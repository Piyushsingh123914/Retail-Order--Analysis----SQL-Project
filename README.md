## Questions

## Basic

* Display each customer's full name with a title (Mr/Ms), with first and last names in upper case, along with their email, creation date and a category: A (created before 2005), B (2005 to 2010) or C (2011 onwards), using `CASE`.
* Display the product class code, class description, count of product types and inventory value (quantity available x price) for each product class, showing only classes with an inventory value above 1,00,000, sorted by inventory value from high to low.
* Display the order ID and volume of the biggest order (by volume) that can fit in carton ID 10.
* Display the customer ID, full name, total quantity and total value (quantity x price) shipped for customers whose payment mode is Cash and whose last name starts with 'G'.
* Display the order ID, customer ID, full name and total quantity of products shipped for even order IDs shipped to addresses whose pincode does not start with '5'.

## Advanced

* Display the product ID, description, quantity available, price, inventory value and new price for products that have not been sold, applying a 20% discount for prices above 20,000, 15% for prices above 10,000 and 10% for prices up to 10,000, sorted by inventory value from high to low.
* Display the customer ID, full name, email, phone and country of customers who have cancelled all the orders they placed, using a subquery.
* Display the shipper name, the city it serves, the number of customers served and the number of consignments delivered to that city for the shipper DHL.
* Display each product's ID, description, quantity available and quantity sold, along with an inventory status (for example "Low inventory, need to add inventory"), using different percentage thresholds for Electronics and Computer, Mobiles and Watches, and the other categories, with a subquery.
* Display the product ID, description and total quantity of products sold together with product ID 201 that were not shipped to Bangalore or New Delhi, sorted by total quantity from high to low, using a subquery.
