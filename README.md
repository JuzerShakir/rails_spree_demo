# Project: Shop You
*An e-commerce demo site built using Spree gem along with ability to checkout products and make payments using Stripe gem. Built on Ruby On Rails*

<div align="center">
  <img src="Images/logo.png" />
</div>


![](https://visitor-badge-reloaded.herokuapp.com/badge?page_id=juzershakir.rails-spree-demo&color=000000&lcolor=000000&style=for-the-badge&logo=Github)


## ❗ Objectives
This web-app must accomplish the following:
- [x] Initialize E-Commerce app with the [Spree Starter]('https://dev-docs.spreecommerce.org/getting-started/installation').
- [x] Add new Products to the site.
- [x] Create new Shipping Category to ship products to customers.
- [x] Create a Taxanomy.
- [x] Create 2 Catergories of products, each categories have 2 sub-categories.
- [x] Create a new Stock Location for products.
- [x] For most of the products create option-types (like: a model of phone can be available in multiple colors in different storage capacity.)
- [x] Customer can then select any single item and add them to cart.
- [x] Customers are able to fill Billing Address form for payment.
- [x] Setup payment method via StripeGateway.
- [x] Specify Country/zone where the product is able to ship.
- [x] Customer can then pay with the currency for country it is able to ship to.
- [x] Payments for orders should be successful with these [test cards specified]('https://stripe.com/docs/testing#cards').

----

## 💎 Required Gems

**This project was built on Ruby version *3.0.2*.**

Additional important gems were added:

|  **Gem Names**  |         **Gem**        |     **Use**            |
| :------------:  |     :------------:     |      :---------:       |
| Spree Frontend  |   spree_frontend       |   For frontend         |
|  Spree Gateway  |   spree_gateway        |    For Payments        |

----

## ⚙️ Setting up a PostgreSQL user

If you don't have a user set on postgres, here's how to set new user:

```bash
sudo -u postgres createuser -s [username]
```
To set a password for this user, log in to the PostgreSQL command line client:
```bash
sudo -u postgres psql
```
Enter the following command to set the password:
```bash
\password your_password
```
Enter and confirm the password. Then exit the PostgreSQL client:
```bash
\q
```

-----

## 📋 Execution

Run the following commands to execute locally:

The following will install required version of ruby (make sure [rvm is installed](https://rvm.io/rvm/install).)

```bash
rvm use 3.0.2
```
```bash
git clone git@github.com:JuzerShakir/rails_spree_demo.git
```
```bash
cd rails_spree_demo
```
```bash
bundle install
```

### 💡 Imp Note:
> In `config/database.yml`, add your own postgresql username and password in the file.

```bash
rails s
```

ENJOY!

-----

To see this web-app up and running without executing above commands locally,
I have deployed it on [Heroku](https://shop-you.herokuapp.com/). The product images will not show up as I have used free Amazon Cloud service which deletes images assets from their servers within 3-4 days.

-----

