## Questions

## Basic

* **** Write a query to display customer full name with their title (Mr/Ms), both first name and last name in upper case, customer email id, customer creation date and display the customer's category after applying the categorization rules below:
  * If customer creation date year < 2005, then Category A
  * If customer creation date year >= 2005 and < 2011, then Category B
  * If customer creation date year >= 2011, then Category C

  Hint: Use a CASE statement; no permanent change in the table is required.
  Tables to be used: ONLINE_CUSTOMER

* **Q3.** Write a query to display Product_class_code, Product_class_description, count of product type in each product class and Inventory Value (product_quantity_avail * product_price). Information should be displayed only for those product_class_code which have an Inventory Value of more than 1,00,000. Sort the output by decreasing Inventory_Value.

  Tables to be used: PRODUCT, PRODUCT_CLASS

* **Q10.** Write a query to display the order_id, customer_id, customer full name and total quantity of products shipped for order ids which are even and shipped to an address where the pincode does not start with "5".

  Tables to be used: ONLINE_CUSTOMER, ORDER_HEADER, ORDER_ITEMS, ADDRESS

* **Q8.** Write a query to display customer id, customer full name, total quantity and total value (quantity * price) shipped where the mode of payment is Cash and the customer last name starts with 'G'.

  Tables to be used: ONLINE_CUSTOMER, ORDER_ITEMS, PRODUCT, ORDER_HEADER

* **Q7.** Write a query to display the order_id and volume of the biggest order (in terms of volume) that can fit in carton id 10.

  Tables to be used: CARTON, ORDER_ITEMS, PRODUCT

## Advanced

* **Q2.** Write a query to display the following information for the products which have not been sold: product_id, product_desc, product_quantity_avail, product_price, inventory value (product_quantity_avail * product_price) and New_Price after applying the discount as per the criteria below. Sort the output by decreasing Inventory_Value.
  * If product price > 20,000, then apply a 20% discount
  * If product price > 10,000, then apply a 15% discount
  * If product price <= 10,000, then apply a 10% discount

  Hint: Use a CASE statement; no permanent change in the table is required.
  Tables to be used: PRODUCT, ORDER_ITEMS

* **Q5.** Write a query to display the shipper name, the city to which it is catering, the number of customers catered by the shipper in the city and the number of consignments delivered to that city for shipper DHL.

  Tables to be used: SHIPPER, ONLINE_CUSTOMER, ADDRESS, ORDER_HEADER

* **Q4.** Write a query to display customer_id, full name, customer_email, customer_phone and country of customers who have cancelled all the orders placed by them (USE SUB-QUERY).

  Tables to be used: ONLINE_CUSTOMER, ADDRESS, ORDER_HEADER

* **Q9.** Write a query to display product_id, product_desc and total quantity of products which are sold together with product id 201 and are not shipped to the cities Bangalore and New Delhi. Display the output in descending order of tot_qty (USE SUB-QUERY).

  Tables to be used: ORDER_ITEMS, PRODUCT, ORDER_HEADER, ONLINE_CUSTOMER, ADDRESS

* **Q6.** Write a query to display product_id, product_desc, product_quantity_avail, quantity sold and show the inventory status of products as per the conditions below (USE SUB-QUERY):
  * For the **Electronics and Computer** categories:
    * if sales till date is zero, show 'No Sales in past, give discount to reduce inventory'
    * if inventory quantity is less than 10% of quantity sold, show 'Low inventory, need to add inventory'
    * if inventory quantity is less than 50% of quantity sold, show 'Medium inventory, need to add some inventory'
    * if inventory quantity is more than or equal to 50% of quantity sold, show 'Sufficient inventory'
  * For the **Mobiles and Watches** categories, the same four messages with these limits:
    * Low: less than 20% of quantity sold
    * Medium: less than 60% of quantity sold
    * Sufficient: 60% or more of quantity sold
  * For the **rest of the categories**, the same four messages with these limits:
    * Low: less than 30% of quantity sold
    * Medium: less than 70% of quantity sold
    * Sufficient: 70% or more of quantity sold
