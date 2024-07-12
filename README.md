
# Wanderlust - Airbnb Clone

## Introduction

Wanderlust is an Airbnb clone built using Express.js, MongoDB, and EJS. This project is part of a series aiming to create a full-fledged vacation rental application. The current version includes basic CRUD operations for managing listings.

## Features

- **Create Listings**: Users can create new property listings.
- **View Listings**: Users can view all available listings.
- **Edit Listings**: Users can edit existing listings.
- **Delete Listings**: Users can delete listings they no longer need.

## Technologies Used

- **Express.js**: For handling server-side logic.
- **MongoDB**: As the database for storing listings.
- **Mongoose**: For object data modeling (ODM).
- **EJS**: For rendering dynamic HTML pages.
- **Method-Override**: To support PUT and DELETE HTTP methods in forms.

## Getting Started

### Prerequisites

Ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/en/)
- [MongoDB](https://www.mongodb.com/)
- [Git](https://git-scm.com/)

### Installation

1. **Clone the repository**:

    ```sh
    git clone https://github.com/yourusername/wanderlust.git
    cd wanderlust
    ```

2. **Install dependencies**:

    ```sh
    npm install
    ```

3. **Start MongoDB**:

    Make sure MongoDB is running on your machine. You can start it using:

    ```sh
    mongod
    ```

4. **Run the application**:

    ```sh
    node app.js
    ```

    The application will be running on `http://localhost:8080`.

## File Structure

```
wanderlust/
├── models/
│   └── listing.js        # Mongoose model for listings
├── views/
│   ├── listings/
│   │   ├── index.ejs     # View for listing all properties
│   │   ├── new.ejs       # View for creating a new listing
│   │   ├── edit.ejs      # View for editing a listing
│   │   └── show.ejs      # View for showing a single listing
│   └── partials/
│       └── header.ejs    # Common header partial
├── app.js                # Main application file
├── package.json          # Project dependencies
└── README.md             # Project documentation
```

## Routes

- **Root Route**: `/`
  - Displays a welcome message.
  
- **Index Route**: `/listings`
  - Lists all property listings.
  
- **New Route**: `/listings/new`
  - Form to create a new listing.
  
- **Create Route**: `/listings`
  - Handles the creation of a new listing.
  
- **Edit Route**: `/listings/:id/edit`
  - Form to edit an existing listing.
  
- **Show Route**: `/listings/:id`
  - Displays details of a single listing.
  
- **Update Route**: `/listings/:id`
  - Handles the update of an existing listing.
  
- **Delete Route**: `/listings/:id`
  - Handles the deletion of a listing.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License.

## Acknowledgements

- Thanks to the open-source community for providing great tools and resources.

---

Feel free to customize it further based on your specific project needs!
