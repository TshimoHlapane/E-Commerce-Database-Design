## 📦 E-commerce Database

This project defines a normalized SQL database schema for an e-commerce platform, supporting product management, inventory, attributes, and variations (e.g., size and color). It's designed to be scalable and modular, accommodating real-world requirements such as stock tracking, dynamic product attributes, and multiple images per product.

## 📁 Database Overview

Database Name: E_commerce

## 🗂️ Tables & Relationships


Table Name	Description
brand	Stores product brand names.
product_category	Defines categories for products (e.g., Electronics, Clothing).
product	Main product entity; links to brand and category.
color	Available color options for products.
size_category	Grouping of sizes (e.g., Clothing, Shoes).
size_option	Specific size values under a size category (e.g., S, M, L).
product_image	Stores product images with URLs.
product_variation	Represents a product’s specific size and color combo.
product_item	Final sellable unit with price and stock information.
attribute_category	Grouping for attributes (e.g., Technical Specs, Fabric Info).
attribute_type	Type of an attribute (e.g., Text, Number).
product_attribute	Stores custom attributes and values per product.
🔗 Key Relationships

product references brand and product_category.
product_item links to product, color, and size_option.
product_variation represents combinations of size and color per product.
product_image enables multiple images per product.
product_attribute allows custom metadata to be stored for each product.
🛠️ Usage

## To use this schema:

Run the CREATE DATABASE E_commerce; command.
Switch to the database with USE E_commerce;
Execute the remaining CREATE TABLE statements in order to set up the schema.
This schema is suitable for:

## E-commerce platforms with extensive product catalogs.
Inventory and variation tracking.
Dynamic attribute-based filtering.

## 📌 Notes

Foreign keys ensure data integrity between related tables.
Designed for extensibility—additional features like orders, users, or reviews can be added seamlessly.