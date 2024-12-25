# DeSerializerNugetAttributes

This repository demonstrates how to read and deserialize sales data from a JSON file into a list of `Sale` objects using `Newtonsoft.Json` in C#. It also includes functionality to display the sale details, including product name, cost, and sale date.

## Prerequisites

Make sure you have the following installed on your machine:

- [.NET SDK](https://dotnet.microsoft.com/download) (any version compatible with your project)
- [Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json/) NuGet package

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/your-username/sales-data-deserialization.git
    ```

2. Navigate to the project directory:

    ```bash
    cd sales-data-deserialization
    ```

3. Install the required NuGet packages:

    ```bash
    dotnet restore
    ```

## Usage

1. Ensure you have a `sales.json` file in the `Archives` folder, formatted as follows:

    ```json
    [
      {
        "Id": 1,
        "Product": "Office Material",
        "Cost": 25.00,
        "SaleDate": "2024-12-25T17:25:06.8154094-03:00"
      },
      {
        "Id": 2,
        "Product": "Software License",
        "Cost": 80.00,
        "SaleDate": "2024-12-25T17:25:06.8154094-03:00"
      }
    ]
    ```

2. Run the application:

    ```bash
    dotnet run
    ```

3. The program will output the sale information to the console in the following format:

    ```
    Id: 1, Product: Office Material, Cost: 25.00, Date: 25-12-2024
    Id: 2, Product: Software License, Cost: 80.00, Date: 25-12-2024
    ```

## Code Structure

- **`Sale` class**: Defines the structure for the sale data with properties such as `Id`, `Product`, `Cost`, and `SaleDate`.
- **`Program.cs`**: Contains the main logic for reading the JSON file, deserializing it, and printing the results.

Steps to Set Up:

Prerequisites: Lists the tools you'll need to run the project.
Installation: Provides step-by-step instructions on how to clone the repository and set up the environment.
Usage: Instructions on how to run the project.
Code Structure: Explains the project structure.
License: Optional section if you'd like to license your code under an open-source license (e.g., MIT).
