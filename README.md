# Public Data Files

This repository hosts public CSV datasets intended for programmatic access by web apps and AI tools.

All files under `/data` are publicly accessible and CORS-enabled.

## Usage

Base URL:  
https://muslimans.netlify.app/data/

Example:  
https://muslimans.netlify.app/data/businesses-ny.csv

## Dataset Schemas

### businesses-ny.csv

| Column     | Description |
|------------|-------------|
| record_id  | Stable unique identifier (never reused) |
| name       | Business name |
| city       | City |
| state      | Two-letter state code |
| category   | Business category |

## Categories

Businesses may belong to **one or more categories**.

When multiple categories apply, they are stored as a
pipe-separated (`|`) list in the `category` column.

### Allowed Category Values

- artist
- autobody
- automotive
- bakery
- barbershop
- butcher
- cafe
- carpet-store
- clothing-store
- convenience-store
- deli
- dessert-shop
- fast-food
- furniture-store
- gift-shop
- graphic-design
- grocery
- hair-salon
- halal-cart
- jewelry-store
- law-firm
- mechanic
- poultry
- restaurant
- retail-store
- retail-supplier
- software-engineering
- towing

New categories may be added in the future.  
Any new category **must be added to this list** and follow
lowercase, hyphenated naming conventions.
