# Data Contract Conformance Check with datacontract-cli

This repository demonstrates how to check that your data delivery conforms to a data contract using the [datacontract.com](https://datacontract.com) CLI.

More details you can find in the LinkedIn post: [Testing Data Contracts with datacontract.com](https://www.linkedin.com/feed/update/urn:li:activity:7375296445676945408/)

## Prerequisites

- Python 3.9+ installed
- Access to your data postgres 

## Setup

1. **Create a virtual environment**  
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```


2. **Install the data contracts CLI**
    ```bash
    pip install --upgrade pip
    pip install uv
    uv pip install -r requirements.txt
    ```

3. **Run the command**
    ```bash
    datacontract test rolling_30_day_orders_postgres.yml
    ```