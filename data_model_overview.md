# data_model_overview.md

# Data Model Overview

## Sales Table

The `sales` table keeps information about every sale, including the product, the customer, and the amount.

| Column | Description |
| --- | --- |
| Transaction Date | Date of purchase |
| Customer ID | Customer identifier |
| Description | Product description |
| Stock Code | Product code |
| Invoice No | An invoice contains multiple products and represents a single checkout |
| Quantity | Quantity of a product purchased |
| Sales | Total amount of a product in a single checkout |
| Unit Price | Unit price of a product |

---

## State Mapping

The `state_mapping` table maps multiple variations of state codes and descriptions to a standardized state code.

| Column | Description |
| --- | --- |
| Order State | State code, description, and all its variations |
| State | A standardized state code |
| Region | Region name |

---

## Product Table

The `product` table keeps product descriptions, landed and shipping costs, weight, and category.

| Column | Description |
| --- | --- |
| Stock Code | Product code |
| Weight | Weight of a single unit |
| Landed Cost | Manufacturer cost plus freight |
| Shipping_Cost_1000_r | Average cost of shipping 1000 miles to customers |
| Description | Most recent product description |
| Category | Product category |

---

## Customer Table

The `customer` table stores customer identifiers and their location information.

| Column | Description |
| --- | --- |
| Customer ID | Customer unique identifier |
| Order City | City |
| Order Postal | Postal code |
| Order State | State |
| Latitude | Latitude of customer location |
| Longitude | Longitude of customer location |