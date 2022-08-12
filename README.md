# [WooCommerce Nextjs React Theme](https://woo-next-imranhsayed.vercel.app/)

> * This is a React WooCommerce theme, built with Next JS, Webpack, Babel, Node, GraphQl

# Features:

1. WooCommerce Store in React( contains: Products Page, Single Product Page, AddToCart, CartPage and Checkout Page with country selection ).
2. SSR
3. SEO friendly
4. Automatic Code Splitting
5. Hot Reloading
6. Prefetching
8. Incremental Static (Re)generation ( Next.js 10 support )
9. GraphQL with Apollo Client
10. Tailwindcss
11. Stripe Checkout ( with Stripe Session and Stripe webhook)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development purposes.

### Installing

`yarn install`
`create .env file`

## Add GraphQl support for WordPress

1. Download and activate the following plugins , in your WordPress plugin directory:

* [wp-graphql](https://github.com/imranhsayed/woo-next/tree/master/wordpress/plugins) Exposes graphql for WordPress ( **Tested with v-1.3.8** of this plugin )
* [wp-graphql-woocommerce](https://github.com/imranhsayed/woo-next/tree/master/wordpress/plugins) Adds Woocommerce functionality to a WPGraphQL schema ( **Tested with v-0.8.1** of this plugin )
* [headless-cms](https://github.com/imranhsayed/woo-next/tree/master/wordpress/plugins) Extends WPGraphQL Schema ( **Tested with v-1.8.0** of this plugin )

* Make sure Woocommerce plugin is also installed in your WordPress site. You can also import default wooCommerce products that come with wooCommerce Plugin for development ( if you don't have any products in your WordPress install ) `WP Dashboard > Tools > Import > WooCommerce products(CSV)`: The WooCommerce default products csv file is available at `wp-content/plugins/woocommerce/sample-data/sample_products.csv`

## Hero Carousel.
To use Hero carousel, create a category called 'offers' from WordPress Dashboard > Products > Categories.
Now create and assign as many child categories to this parent 'offers' category with name, description and image.
These Child categories data will automatically be used to create hero carousel on the frontend.
