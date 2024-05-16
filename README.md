# Toy Trading Engine

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Configuration](#configuration)
6. [API Endpoints](#api-endpoints)
7. [Troubleshooting](#troubleshooting)
8. [Contributing](#contributing)
9. [License](#license)
10. [Contact](#contact)

## Introduction
The Toy Trading Engine is a simplified simulation of a trading engine designed for educational purposes. It demonstrates the core functionalities of a trading system, including order placement, order matching, and trade execution. This project is implemented in C++.

## Features
- **Order Placement**: Users can place buy and sell orders.
- **Order Matching**: The engine matches buy and sell orders based on price and time priority.
- **Trade Execution**: Executes trades when orders are matched.
- **Order Book Management**: Maintains an order book for buy and sell orders.
- **Transaction History**: Keeps a record of executed trades.

## Installation
To install and run the Toy Trading Engine locally, follow these steps:

1. **Clone the Repository**
    ```bash
    git clone https://github.com/yourusername/toy-trading-engine.git
    cd toy-trading-engine
    ```

2. **Install Dependencies**
    Ensure you have a C++ compiler and CMake installed on your system. If not, install them as follows:
    
    - **Ubuntu/Debian**
        ```bash
        sudo apt-get install build-essential cmake
        ```
    - **MacOS**
        ```bash
        brew install cmake
        ```

3. **Build the Project**
    ```bash
    mkdir build
    cd build
    cmake ..
    make
    ```

4. **Run the Application**
    ```bash
    ./toy_trading_engine
    ```

## Usage
1. **Place Orders**
    - Users can place buy or sell orders through the command line interface or via API if implemented.

2. **Order Matching**
    - The engine will automatically match and execute orders based on price and time priority.

3. **View Orders and Trades**
    - Users can view the current order book and transaction history through the command line interface or API.

## Configuration
Configure the application by modifying the configuration file `config.json` in the root directory:

```json
{
    "database_url": "your-database-url",
    "port": 3000,
    "secret_key": "your-secret-key"
}
```

## API Endpoints
Below are the primary API endpoints available in the Toy Trading Engine (if API support is implemented):

- **Order Endpoints**
    - `POST /api/orders`: Place a new order.
    - `GET /api/orders`: Retrieve the current order book.
    - `GET /api/orders/:id`: Get details of a specific order.

- **Trade Endpoints**
    - `GET /api/trades`: Retrieve a list of executed trades.
    - `GET /api/trades/:id`: Get details of a specific trade.

## Troubleshooting
If you encounter issues while using the Toy Trading Engine, try the following steps:

1. **Check Logs**
    - Review application logs for any error messages.

2. **Verify Configuration**
    - Ensure all required configuration settings are correctly set in `config.json`.

3. **Database Connectivity**
    - Check if the database is running and accessible.

4. **Common Issues**
    - Build errors: Ensure all dependencies are correctly installed and try rebuilding the project.
    - Runtime errors: Check for any missing configuration or database connection issues.

## Contributing
We welcome contributions to the Toy Trading Engine! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License
The Toy Trading Engine is licensed under the [MIT License](LICENSE).

## Contact
For any questions or feedback, please contact us at [support@toytradingengine.com](mailto:support@toytradingengine.com).

Thank you for using the Toy Trading Engine! We hope it serves as a valuable educational tool.
