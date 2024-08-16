# Store Management System

## Overview

The **Store Management System** is a software application designed to manage retail store operations with Java.\
The system facilitates the storage, retrieval, and management of essential data, including product information, customer details, sales transactions, and inventory levels.

## Features

- **Product Management**: 
  - Add new products to the inventory.
  - Remove existing products from the inventory.
  - Update the quantity of products in stock.
  - View detailed information about each product, including orders and profits.

- **Order Management**: 
  - Add new orders to products.
  - Remove the last order from a product.
  - View orders associated with specific products.
  - Automatically calculate and display the profit from each order.

- **Backup and Restore**: 
  - Create a backup of the current state of the system.
  - Restore the system to the last backup.

- **Auto-Generation**: 
  - Automatically create a set of sample products and orders for testing.

## Getting Started

### Prerequisites

To run this project, you need the following:

- **Java Development Kit (JDK)** - Version 8 or higher
- **SQL Database** - For storing product and order information (integration with Java backend is required)
- **IDE** - Such as IntelliJ IDEA, Eclipse, or NetBeans

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/factory-managment.git
   ```

2. Open the project in your preferred IDE.

3. Set up your SQL database and configure the connection settings in the project.

4. Compile and run the project.

### Usage

1. Run the application:

   ```bash
   java -jar StoreManagementSystem.jar
   ```

2. Follow the on-screen prompts to manage your store’s inventory and orders.

3. Use the menu options to:
   - Automatically create products and orders
   - Manually add, update, or remove products
   - Manage orders for specific products
   - Backup or restore the system state

### Main Menu Options

- **1) Automatic Create**: Automatically generates a set of products and orders for testing.
- **2) Add New Product**: Allows the user to add a new product to the inventory.
- **3) Remove Product**: Removes a product from the inventory by serial number.
- **4) Update Product's Amount**: Updates the stock amount of a specific product.
- **5) Add an Order for a Product**: Adds a new order for a specified product.
- **6) Remove the Last Order**: Removes the last order placed on a product.
- **7) Review a Product's Details**: Displays detailed information about a specific product, including all orders and profit calculations.
- **8) Review All Products**: Displays a summary of all products in the inventory.
- **9) Print a Product's Orders**: Prints all orders associated with a specific product.
- **10) Restore Last Backup**: Backs up the current state or restores the last backup.
- **E) Exit**: Exits the program.

### Classes and Design Patterns

- **storeFacade**: Implements the Facade pattern, providing a simplified interface to manage the store's operations.
- **Memento Pattern**: Used for backup and restore functionality.
- **Factory Pattern**: Different product types are created using Factory classes (`soldthroughwebsiteFactory`, `soldinStoreFactory`, `SoldToWholesellersFactory`).


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
