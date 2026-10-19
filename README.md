# Shopping-cart
# Online Shopping Cart (Python)

A command-line shopping cart built for my Python programming course at DeVry University (Project 7.1.1, scored 105/105). Users can add, remove, and change the quantity of items, then view an itemized receipt with the cart total.

## Features

- Add items with a name, price, and quantity
- Remove items by name
- Change the quantity of an item already in the cart
- Print an itemized cart with the total item count and total cost
- Input validation on the menu (keeps prompting until a valid option is entered)

## How to run

Requires Python 3.

```bash
python main.py
```

## Example session

What it looks like in a terminal (user input shown after each prompt):

```
Enter customer's name: John Doe
Enter today's date: February 1, 2025

Customer name: John Doe
Today's date: February 1, 2025

MENU
a - Add item to cart
r - Remove item from cart
c - Change item quantity
o - Output shopping cart
q - Quit

Choose an option:
a
ADD ITEM TO CART
Enter the item name: Nike Romaleos
Enter the item price: 189
Enter the item quantity: 2

...

Choose an option:
o
OUTPUT SHOPPING CART
John Doe's Shopping Cart - February 1, 2025
Nike Romaleos 2 @ $189 = $378
Chocolate Chips 5 @ $3 = $15
Powerbeats 2 Headphones 1 @ $128 = $128
Number of Items: 8

Total: $521
```

## Design

The program is built around two classes:

| Class | Responsibility |
|---|---|
| `ItemToPurchase` | Stores an item's name, price, and quantity; prints its line cost |
| `ShoppingCart` | Stores the customer name, date, and list of items; handles add, remove, modify, and totals |

The menu is handled by two functions: `print_menu()` displays the options, and `execute_menu()` runs the action for the chosen option.

## What I practiced

- Object-oriented programming: classes, constructors with default values, and methods
- Managing a list of objects (searching, updating, and removing by attribute)
- Menu-driven program flow with input validation
- Formatted string output with f-strings
shopping cart project
