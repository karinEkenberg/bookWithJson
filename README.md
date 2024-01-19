# Readme

## Introduction
This is a simple C# console application that reads and displays information from a JSON file containing book data. The application utilizes the Newtonsoft.Json library for JSON deserialization.

## Prerequisites
Before running the code, make sure you have the Newtonsoft.Json library installed in your Visual Studio Code environment.

To install the library, you can use the following command in the terminal inside Visual Studio Code:
```bash
dotnet add package Newtonsoft.Json
```

## Usage
1. Download and install the Newtonsoft.Json library using the above command.
2. Make sure you have a valid JSON file named `data.json` with the required book information. If not, you can create your own file or use the provided one.
3. Run the application in Visual Studio Code or your preferred C# development environment.

## Code Explanation
### Classes
- **Book**: Represents the structure of a book with properties for title, author, and code.
- **Root**: Represents the root object containing a list of books.

### Methods
- **checkInputs**: Checks if the input array is null or empty and throws exceptions accordingly.
- **importJSON**: Deserializes the content of the `data.json` file into the `Root` object using Newtonsoft.Json.
- **DisplayBookInfo**: Displays information about a book on the console.

### Main Method
- The `Main` method serves as the entry point for the application.
- It attempts to import and display book information from the JSON file.
- If successful, it iterates through each book, displaying its details.
- If no data is found in the JSON file, it prints a message indicating that.
- If an error occurs during the process, it catches the exception and prints an error message.

## Note
Ensure that the `data.json` file is present and correctly formatted with the necessary book information for the program to execute successfully.
