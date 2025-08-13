# Product-List
1. HTML Structure
<!DOCTYPE html>: Declares the document type.

<head>: Contains metadata, page title, and CSS styles.

<body>: Contains:

A heading (<h2>)

Filter inputs: a search bar, brand dropdown, and category dropdown

A table that displays products fetched from an API

2. CSS Styling
Defines a clean, modern layout with:

Centered title and filters

Styled table with hover effects

Product images and formatted prices

3. JavaScript Functionality

fetchProducts():
Fetches product data from https://dummyjson.com/products?limit=100

Saves the data to productsData

Calls populateFilters() and displayProducts()

 populateFilters(products):
Gets all unique brands and categories from the product list

Populates the <select> filters with those options

displayProducts(products):
Dynamically creates table rows from product data

Clicking a row redirects to a detailed product page (product.html?id=product.id)

applyFilters():
Filters products based on search input, selected brand, and category

Displays only the filtered products

 Event Listeners:
Runs filtering function when user types in the search box or changes dropdowns

