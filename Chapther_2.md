*Learn Odoo*

**Chapther 2**

# Installing Your First Application

*... same notes that I image useful for me...*

## Gathering requirements

### Implementing Odoo using a modular approach

To manage your Odoo implementation, **you must begin with planning the modules with which you will work first**.

Odoo allows you to install just what you need now and then install additional Odoo modules as you better define your requirements.

>When implementing Odoo for your organization, you will also want to create a basic requirements document.

## Creating a new database in Odoo

### Managing databases in Odoo

The database management interface allows you to perform basic database management tasks such as **backing** up or **restoring** a database.

#### Set up multiple databases

It is also possible to set up multiple databases under the same installation of Odoo. *For instance*, in the future, you may want to install another database that loads demonstration data and may be used **to install modules simply for testing purposes**.

>You can access the database management interface directly by going to the **/web/database/manager path**

## Installing the Sales application

### Knowing the basic Odoo interface

**Discuss messaging app** where your inbox and other communication activities are located.

Notice the **small purple teardrop** that provides *helpful tips*.

**Sales application** there is a brand new onboarding panel to configure the application.

Working from left to right, *like as a wizard*, we can see that it starts with the *Company Data*. You then pick a **Quotation Layout** to customize the look of your quotations and sales orders.

#### Using multiple contacts and addresses
An individual customer can have multiple contacts and addresses.

#### Editing customer Sales & Purchases

The available options in the customer Sales & Purchases page are as follows:
- Is a Customer;
- Salesperson (*Customer Relationship Management (CRM)*);
- Internal Reference;
- Is a Vendor;

>Odoo uses a **common database** to store customer and supplier records.

## Entering a product in Odoo

### Creating products in Odoo

#### Can be sold
You can use Can be Sold to remove products from showing up on product lists.

#### Can be purchased
This will play an important function when we get to *Chapter 4 , Purchasing with Odoo*.

#### Product type
- Service;
- Consumables;

**Service product** types will not create procurement (*approviggionamento*) in purchase orders.
**Consumables** are products that you actually sell and can be configured to generate purchase orders.

#### Internal reference
It can be field blank.

#### Sale price

#### The Cost price
It can be utilized for simple profit margin calculations.

### Entering a product Invoicing page
By default, Odoo has set up a tax of 15% for both our **Customer Taxes** and our **Vendor Taxes**. However, there will be times when you have a product that has a specific tax.

#### Invoicing policy
By default, Odoo configures invoicing so that the line items of the invoice will be created depending on the ordered quantities from the sales order.


---

[![Francesco Dattolo](https://i0.wp.com/www.francescodattolo.it/wp-content/uploads/2019/09/cropped-francescodattolo-free_hand-logo-1.png)](https://francescodattolo.it)

*Francesco Dattolo*

*2108181113*