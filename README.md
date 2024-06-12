# Book Management Application

This is an ASP.NET Core MVC application for managing a collection of books. The application demonstrates the use of the MVC pattern, Entity Framework Core, and the Repository pattern.

## Features

- Add new books
- Update existing books
- List all books
- Delete books

## Technologies Used

- ASP.NET Core MVC
- Entity Framework Core
- Repository Pattern
- SQL Server

## Getting Started

Follow these instructions to get the application up and running on your local machine.

### Prerequisites

- .NET 6.0 SDK or later
- SQL Server (LocalDB or full version)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/krispyarena/books-crud-app.git
   cd books-crud-app
   ```

2. **Set up the database:**

   Update the connection string in `appsettings.json` to point to your SQL Server instance.

   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=KRISPY\\mssqllocaldb;Database=BookManagementDb;Trusted_Connection=True;MultipleActiveResultSets=true"
   }
   ```

3. **Run database migrations:**

   Open a terminal in the project directory and run the following commands:

   ```bash
   dotnet ef migrations add InitialCreate
   dotnet ef database update
   ```

4. **Run the application:**

   ```bash
   dotnet run
   ```

5. **Access the application:**

   Open your web browser and navigate to `https://localhost:5001` or `http://localhost:5000`.

## Project Structure

- **Controllers:** Handles the incoming HTTP requests and sends the responses.
- **Models:** Contains the business entities (e.g., Book) and the DbContext for EF Core.
- **Views:** Contains the Razor views for displaying the data.
- **Repositories:** Implements the repository pattern for accessing data.

## Usage

### Adding a New Book

1. Navigate to the "Add Book" page.
2. Fill in the book details.
3. Click the "Save" button.

### Updating an Existing Book

1. Navigate to the "List Books" page.
2. Click the "Edit" button next to the book you want to update.
3. Update the book details.
4. Click the "Save" button.

### Listing All Books

1. Navigate to the "List Books" page.
2. View the list of all books in the database.

### Deleting a Book

1. Navigate to the "List Books" page.
2. Click the "Delete" button next to the book you want to delete.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

```

Replace `https://github.com/krispyarena/book-management-app.git` with the actual URL of your GitHub repository. This README file provides a clear and concise guide for anyone who wants to understand, set up, and contribute to your book management application.
