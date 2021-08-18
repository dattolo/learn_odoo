*Learn Odoo*

**Chapther 15**

# Discovering Custom Odoo Modules

While Odoo has a lot of built-in and community modules, it is inevitable that there will be quite a few businesses that will have requirements that will be difficult to meet with the modules that are currently available.

Topics:
- Learning the basic structure of an Odoo module;
- Using a module to add additional fields to your Odoo system;
- Extending the views in your Odoo instance to include new fields;
- Making changes to the available states to use in an Odoo workflow;


Before you go down the path of writing custom Odoo modules, it is important that you are absolutely sure that your business requirements are clear and you have thoroughly explored all of the options available in Odoo.


## Exploring the Odoo application and module directory

In Odoo development, we can sometimes refer to custom applications and modules interchangeably.

## Building our first Odoo module

## Using Odoo to create websites and web services

Let's see how we can create a simple web service that displays the rush orders on a page.

To test our controller and make sure it is functioning properly, place the following code in the **controller.py** file to create a simple output:
```python
from odoo import http

class Web_RushOrders(http.Controller):
    @http.route('/orders/rush/', auth='public')

    def index(self, **kw):
        Orders = http.request.env['sale.order']

        return http.request.render('silkworm.index', 
                {'rushorders': Orders.search([('rush','=',True)])}
            )
        #return "Rush Orders"
```

**template.xml**

```xml
<odoo>
    <data>
        <template id="index">
            <title>Rush Orders</title>

            <table>
                <t t-foreach="rushorders" t-as="rushorder">
                    <tr>
                        <td><t t-esc="rushorder.name"/></td>
                        <td><t t-esc="rushorder.daterequired"/></td>
                    </tr>
                </t>
            </table>

        </template>
    </data>
</odoo>
```

## Integrating with the Odoo API

The API is also quite useful for **data migration**. 

### Connecting to the API

Accessing the API is relatively easy. 

```python
import xmlrpclib
url = http://localhost:8069
db = SILK-DEV
username = 'admin'
password = 'admin'

info = xmlrpclib.ServerProxy(
    'https://localhost:8089/start').start()

url, db, username, password = \
info['host'], info['database'], info['user'], info['password']
```

### Filtering and returning records through the API

We can use the same **domain filters** that we used in filtering *rush orders*, in order to use the **API** to return a list of sale order IDs that match as showing in the following snippet:

```python
models.execute_kw(db, uid, password,
    'sale.order', 'search',
    [["[('x_rush','=',True),('state','=','progress')]])
```

### Using the search_read method

While the preceding code only returns the IDs of the records, the new Odoo API allows you to both search and read the actual fields from the model with one single API call. Here, we return some fields from the sales order header as shown in the following snippet:

```python
models.execute_kw(db, uid, password,
    'sale.order', 'search_read',
    [[['x_rush, '=', True], ['state', '=', 'done']]],
    {'fields': ['name', 'country_id', 'comment'], 'limit': 5})
```


---

[![Francesco Dattolo](https://i0.wp.com/www.francescodattolo.it/wp-content/uploads/2019/09/cropped-francescodattolo-free_hand-logo-1.png)](https://francescodattolo.it)

*Francesco Dattolo*

*2108181222*