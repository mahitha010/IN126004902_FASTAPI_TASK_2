# FastAPI Internship Assignment

## Intern Information

**Intern ID:** IN126004902
**Module:** FastAPI – Day 2 Assignment

## Overview

This repository contains the implementation of the FastAPI internship assignment. The project demonstrates the development of RESTful APIs using FastAPI, including the use of query parameters, path parameters, request validation with Pydantic, and basic business logic for handling product data, customer feedback, and order processing.

## Implemented Features

### 1. Product Filtering API

**Endpoint:** `GET /products/filter`
Allows users to filter products using query parameters such as category, minimum price, and maximum price.

### 2. Product Price API

**Endpoint:** `GET /products/{product_id}/price`
Returns only the name and price of a specific product based on the provided product ID.

### 3. Customer Feedback API

**Endpoint:** `POST /feedback`
Accepts customer feedback and validates the input using Pydantic models. Feedback includes customer name, product ID, rating, and an optional comment.

### 4. Product Summary Dashboard

**Endpoint:** `GET /products/summary`
Provides a summary of the product dataset including:

* Total number of products
* In-stock and out-of-stock counts
* Most expensive and cheapest products
* Available product categories

### 5. Bulk Order Processing API

**Endpoint:** `POST /orders/bulk`
Handles bulk orders from companies, validates product availability, processes valid items, reports failed items, and calculates the final order total.

## Technologies Used

* **Python**
* **FastAPI**
* **Uvicorn**
* **Pydantic**

## Project Structure

IN126004902_FASTAPI
  ├── main.py
  ├── Q1_Output.png
  ├── Q2_Output.png
  ├── Q3_Output.png
  ├── Q4_Output.png
  └── Q5_Output.png

## Running the Application

Install required dependencies:

pip install fastapi uvicorn

Start the FastAPI server:

uvicorn main:app --reload

## Notes

All endpoints were tested using Swagger UI, and screenshots of the outputs are included in this repository as required by the assignment submission guidelines.
