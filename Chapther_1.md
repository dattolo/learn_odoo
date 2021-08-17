*Learn Odoo*

**Chapther 1**

# Setting Up Odoo 12

*... same notes that I image useful for me...*

## Introducing the PostgreSQL database

Like most **ERP systems**, Odoo has specific database requirements: in this case, **PostgreSQL**. PostgreSQL is an open source, cross-platform Object Relational Database Management System (**ORDMS**). While not popular on the scale of Microsoft SQL Server or MySQL, PostgreSQL is an *enterprise-class database server* with many advanced features. In fact, PostgreSQL stacks up very well against far more expensive databases such as Microsoft
SQL Server and Oracle Database.

## Writing code with Python

The primary programming language of Odoo is **Python**.


*Starting in Odoo 11, Odoo began using Python 3.5 instead of Python 2.7.*

## Following the Model-View-Controller design

Odoo is built upon a **Model-View-Controller (MVC)** architecture. One of the primary goals of this architecture is to separate the visual display of the information from the business rules and management of the underlying data.

*Today, it is common to have many different client applications sharing the same underlying data.*

### Designing models
The model is essentially the data that makes up your Odoo installation, which is stored in the PostgreSQL database.

### Rendering views

Each view in Odoo is defined in XML documents. *The Odoo framework is responsible for rendering these view files in a web browser.*

### Authoring controllers

The *controller component* of the architecture is where the **business logic and workflow rules** of the Odoo application are applied.

## Introducing Ubuntu

Ubuntu (pronounced *oo-BOON-too*) is a very popular open source **OS based on the Linux kernel**.

### Choosing an Ubuntu Odoo installation
There are several reasons why this is true:
- **Ubuntu is the primary target platform**;
- **Ubuntu is open source**;
- **Ubuntu has additional scalability options**;
- **Ubuntu has strong community support for Odoo**: The fact is that *a vast majority of the production installations of Odoo are running under Ubuntu*.




---

[![Francesco Dattolo](https://i0.wp.com/www.francescodattolo.it/wp-content/uploads/2019/09/cropped-francescodattolo-free_hand-logo-1.png)](https://francescodattolo.it)

*Francesco Dattolo*

*2108101424*