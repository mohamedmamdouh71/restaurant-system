# Restaurant Management System — Maidan POS

A full restaurant front-of-house system in a single HTML file. No build step, no server: open `index.html` and it runs.

Arabic first with full right-to-left layout and an English toggle. Prices use Western digits; money in Egyptian pounds, with VAT and service charge applied per order type.

## What it does

- **Floor** — table map by area (indoor / terrace) with live status: free, occupied, ready to serve. Each table shows how long it has been open and the running total. Tap a free table to open an order.
- **Order screen** — pick dishes by section or search, change quantities, add kitchen notes ("no onions"), then send to the kitchen. Subtotal, service, VAT and delivery are worked out automatically.
- **Takeaway & delivery** — tickets with the customer and address attached.
- **Kitchen display** — tickets in three columns (new, cooking, ready) with elapsed time, turning red when a ticket is late. Sends "ready to serve" back to the floor.
- **Menu** — sections, dishes, prices, station (grill / kitchen / drinks) and the recipe behind each dish.
- **Inventory** — ingredients with stock levels and par levels. Sending a dish to the kitchen deducts its recipe from stock, and low or out-of-stock ingredients raise an alert.
- **Customers** — delivery records with address, order history and total spent.
- **Reports** — today's sales, order count, average bill, last 7 days, split by order type, best sellers, payment methods and busiest hours.
- **Payment** — cash with a keypad and change calculation, card, InstaPay or Vodafone Cash, plus a printable receipt.

## Data

This is a prototype. Everything is saved in the visitor's own browser (`localStorage`); nothing is shared between devices and nothing reaches a server. It opens with a sample Egyptian menu, tables, ingredients and a week of sales history, all of which can be cleared in Settings.

For real use in a restaurant, the next step is a database, staff logins per waiter, and a printer connection.
