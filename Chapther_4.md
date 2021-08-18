*Learn Odoo*

**Chapther 4**

# Purchasing with Odoo

*... same notes that I image useful for me...*

The core of the **Enterprise Resource Planning (ERP) systems** is purchasing workflow.

- Examining a typical purchasing process for a business;
- Setting up your vendors and warehouse locations;
- Entering a quote and turning it into a purchase order;
- Receiving products from your vendors;
- Paying invoices;
- Understanding units of measure for placing bulk orders;

## Understanding the overall purchasing process

A purchasing system requires several steps, and initially, it can be confusing for people who are new to ERP systems.

The steps of purchasing:
- Setting up a vendor;
- Setting up warehouse locations;
- Generating quotations and purchase orders;
- Receiving the product;
- Settling the invoice;

### Setting up a vendor
Sometimes, vendors are also referred to as suppliers.

**Odoo, it is completely possible to create a product and sell it without implementing apurchasing system.**

Odoo maintains core customer, employee, and vendor records all in the same model, named *res.partners*.

Odoo distinguishes between customers, vendors, and those who are both, with the use of the **Is a Customer** and **Is a Vendor** checkboxes.


### Setting up warehouse locations

Once you have decided to start using Odoo to purchase your products, you will need to set up locations to receive them from.


### Generating quotations and purchase orders

To acquire the raw product, you will need to create **Requests for Quotations** (richieste di preventivo) and/or **Purchase Orders** (ordini di acquisto) to send to your **vendors** (venditore).

In **purchasing**, these are the documents you create that **tell the vendors which products you require, the quantity in which you require them, and what you expect to pay for those products**.

Often, this process is referred to as **procurement**.

### Receiving the product

When the product has been received, you are ready to create a manufacturing order.

### Settling the invoice

When an invoice is received, it is essential to compare it to the purchase order for accuracy. Any discrepancies between the purchase order and invoice must be resolved before the invoice is paid.



---

[![Francesco Dattolo](https://i0.wp.com/www.francescodattolo.it/wp-content/uploads/2019/09/cropped-francescodattolo-free_hand-logo-1.png)](https://francescodattolo.it)

*Francesco Dattolo*

*2108101424*