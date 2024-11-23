# DSA LAB Project 1
# E-Commerce Product Recommendation System

![C++](https://img.shields.io/badge/language-C++-blue.svg)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies and Data Structures Used](#technologies-and-data-structures-used)
- [Code Overview](#code-overview)
- [Usage](#usage)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## Introduction

The **E-Commerce Product Recommendation System** is a C++ application that reads product data from a CSV file and provides various operations to filter, sort, and recommend products based on user interactions. This recommendation system allows users to perform product searches with autocomplete, get top product suggestions based on views or prices, and more.

## Features

- **Display All Products:** View a comprehensive list of all products available in the CSV data.
- **Top K Products by Views or Price:** Identify and display the top K products based on either views or price.
- **Price Range Recommendations:** Get product recommendations within a specified price range.
- **Filter by Category or Company:** Narrow down products based on their category (e.g., Cars) or the company (e.g., Tata Motors).
- **Search with Autocomplete:** Quickly search for products using name prefixes with real-time suggestions.
- **Sorting Options:** Sort products by price or views in both ascending and descending orders.
- **Error Handling:** Handles invalid data from CSV files and user input gracefully.

## Technologies and Data Structures Used

- **C++**: Core programming language used for developing the application.
- **Data Structures**:
  - **Heap (Priority Queue)**: Used for efficiently retrieving the top K products by views or price.
  - **Hash Map (Unordered Map)**: Facilitates quick access to product data for autocomplete and other operations.
  - **Arrays & Vectors**: Used for managing collections of products and iterating through product lists.
  - **Trie**: Implements an autocomplete functionality for searching products based on name prefixes.
  - **Binary Search Tree (BST)**: Used for efficiently managing product data based on price, allowing quick retrieval of products within a specific price range.

## Code Overview

The code is divided into several parts to perform different operations efficiently:

- **Product Struct**: This struct holds information about each product, including its ID, name, company, category, price, and views.

- **Trie and TrieNode**: The **Trie** data structure helps to implement the autocomplete functionality for product searches by prefix. Each node stores a reference to its children and products associated with that prefix.

- **ProductBST**: This **Binary Search Tree** (BST) is used to organize products based on their price. It allows for efficient insertion and retrieval of products within a specific price range.

- **Priority Queue (Heap)**: Heaps are used to efficiently get the top K products by views or price. This allows for quick identification of popular or expensive products.

- **Filtering and Sorting**:
  - **Category and Company Filters**: Users can filter products based on the given category or company.
  - **Sorting**: Products can be sorted based on price or views, in ascending or descending order.

- **File Handling**:
  - The code reads product data from a CSV file (`ecom.csv`) and uses string manipulation techniques to parse the data, validate it, and create `Product` instances.
  - Proper error handling is implemented to manage invalid or incomplete data.

## Usage

Upon running the program, you will be presented with a console-based menu with the following options:
- Show All Products
- Show Top K Products by Views
- Show Top K Products by Price
- Recommend Products in Price Range
- Filter Products by Category
- Filter Products by Company
- Search Products by Name (with Autocomplete)
- Sort Products
- Exit Enter choice:


### Menu Options Explained

1. **Show All Products**: Displays a list of all products loaded from the CSV file.

2. **Show Top K Products by Views**:
   - Enter the value of `K` (e.g., `5`) to view the top 5 most viewed products.
   
3. **Show Top K Products by Price**:
   - Enter the value of `K` to view the top `K` products with the highest prices.

4. **Recommend Products in Price Range**:
   - Enter a lower and an upper price limit, and the system will display products that fall within this price range.

5. **Filter Products by Category**:
   - Enter a product category (e.g., "Cars") to filter products belonging to that category.

6. **Filter Products by Company**:
   - Enter a company name to filter products produced by that company (e.g., "Tata Motors").

7. **Search Products by Name (with Autocomplete)**:
   - Enter a product name prefix, and the system will suggest products that match the prefix. This is powered by the Trie data structure.

8. **Sort Products**:
   - Offers sorting by price or views, in ascending or descending order, based on the user's preference.

9. **Exit**: Closes the application.

### Example Usage

1. **Display All Products**:
   - Select option `1` to view all the products, including their details such as Product ID, Name, Company, Category, Price, and Views.

2. **Top K Products by Views**:
   - Select option `2` and enter the value of `K` to view the top `K` products with the most views.

3. **Autocomplete Search**:
   - Select option `7`, enter a prefix such as `"Ta"`, and the system will display all products that match this prefix (e.g., "Tata Motors Cars 1").

## Contact

- **Your Name**
- **Email:** your.email@example.com
- **GitHub:** [yourusername](https://github.com/yourusername)

## Acknowledgments

- [C++ Documentation](https://cplusplus.com/doc/tutorial/)
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)
- [Awesome C++](https://github.com/fffaraz/awesome-cpp) - A curated list of awesome C++ frameworks, libraries, and resources.

---



