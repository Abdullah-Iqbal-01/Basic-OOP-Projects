# E-commerce Platform

Welcome to the E-commerce Platform! This system allows users to browse and purchase products, manage their shopping cart, and place orders with ease. It also provides functionality for admins to manage products, view orders, and track inventory.

## Features
- **Product Management**: Add, remove, and update product details.
- **Cart System**: Add products to the cart with customizable quantities.
- **Order Management**: Place, view, and cancel orders.
- **Stock Management**: Automatically update stock levels when products are purchased.
- **User Management**: Handle customer details, order statuses, and payment methods.

## Technologies Used
- **Python**: For backend functionality and business logic.
- **Object-Oriented Programming (OOP)**: Clean and modular design using classes and objects.
- **Data Management**: Manage cart items, orders, and product stock efficiently.

## Getting Started
To run the platform, simply create an instance of the `Cart`, `Product`, and `Order` classes, and interact with the methods provided to manage products and orders.

```python
# Example of creating a product and adding it to a cart
product = Product(1, "Product 1", "Description 1", 10.0, 100, "Category 1")
cart = Cart()
cart.add_product(product, 2)

# Example of placing an order
order = Order(1, cart, 20.0, "John Doe", "123 Main St", "pending", "Cash on Delivery")
order.place_order()
order.view_order_details()
```

## Contributing
Feel free to fork this repository, create issues, and submit pull requests with any improvements or fixes.

