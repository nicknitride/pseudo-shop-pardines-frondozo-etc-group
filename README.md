# Pseudo Shop - A Git Collaboration Simulation

This repository contains the work for the FECP5 Final Exercise, a team project focused on simulating professional software development workflows using Git. The primary goal of this project was to practice collaboration, branch management, and conflict resolution.

**Note:** All code in this repository is written in a `.pseudo` format. The focus was on the development *process*, not on creating a functional application.

### Team Members

* **Ivan Frondozo**
* **Jaime Manalo**
* **Nicholo Pardines**
* **Paolo Flores**
* **Johnvee Mandal** 

### Project Overview

The simulation involved implementing four core features for an e-commerce platform called "Pseudo Shop." The team used a **Feature Branch Workflow**, where each feature was developed in an isolated branch before being merged into the `main` branch.

#### Features Implemented:

1.  **Product Filtering:** A function to filter products based on various attributes (`filter_products`).
2.  **User Authentication:** Functions to handle user registration and login (`create_user`, `login_user`).
3.  **Product Management:** A system for adding products to an in-memory list (`add_product`).
4.  **Storefront Display:** Logic to display product information in a structured format (`display_products`).

A key requirement of the project was to intentionally create and resolve a **merge conflict** to practice this common collaborative challenge.

### Repository Structure

* `product_model.pseudo`: Contains the data structures and logic for managing products.
* `store_view.pseudo`: Handles the logic for displaying products and the storefront.
* `user_controller.pseudo`: Contains the functions related to user registration and login.
* `retrospective.md`: A detailed report answering reflection questions about the team's process, challenges, and learnings.

This project demonstrates a complete, simulated development cycle, from branching and feature implementation to conflict resolution and final merging.