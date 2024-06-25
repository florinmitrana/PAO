# Stock and Cryptocurrency Brokerage System

## Overview
This project is a Java-based backend system designed for a stock and cryptocurrency brokerage and investment platform. The application manages various financial assets, transactions, users, and brokers, providing essential services such as buying and selling stocks, managing portfolios, and calculating broker commissions.

## Features
- **Manage Financial Assets**: Add, update, delete, and view details of stocks (`Actiune`) and cryptocurrencies (`Criptomoneda`).
- **User Management**: Create, update, delete, and retrieve user information.
- **Transaction Handling**: Perform and manage transactions involving stocks and cryptocurrencies.
- **Portfolio Management**: Calculate the total value of user portfolios and display holdings.
- **Broker Services**: Manage brokers and calculate their commissions based on transactions.
- **Dividend Management**: Handle and calculate dividends for stocks.

## Database
The application uses PostgreSQL for storing data related to users, transactions, stocks, cryptocurrencies, and brokers.

## Project Structure
- `model`: Contains the data models for the application, including `Actiune`, `Criptomoneda`, `Dividend`, `Transaction`, `Portofoliu`, `PortofoliuCrypto`, `Utilizator`, and `Broker`.
- `Implementation`: Contains service classes that handle database operations for different entities, including `ActiuneService`, `TransactionService`, `UtilizatorService`, and `BrokerService`.

## Usage
1. **Database Setup**: Ensure you have a PostgreSQL database running. Update the database connection parameters in the `Main` class:
    ```java
    String url = "jdbc:postgresql://localhost:5432/postgres";
    String user = "Enter your database user";
    String password = "Enter your database password";
    ```
2. **Run the Application**: Execute the `Main` class to interact with the system. The `Main` class demonstrates various operations, including adding assets, performing transactions, managing users, and calculating portfolio values.
