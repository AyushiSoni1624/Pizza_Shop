# Pizaa Shop

## Overview

Pizaa Shop is a MERN stack application designed to manage a pizza shop. It features two main components: the Client and the Server. The Client allows customers to browse the menu, place orders, and track their orders. The Server handles user authentication, order processing, and data management.

## Project Structure

```
pizaa_shop/
├── client/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.js
│   │   ├── index.js
│   ├── package.json
├── server/
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   ├── package.json
├── .gitignore
├── README.md
```

## Prerequisites

- Node.js
- MongoDB

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/pizaa_shop.git
cd pizaa_shop
```

### 2. Setting Up the Client

Navigate to the `client` directory and install the dependencies.

```bash
cd client
npm install
```

Create a `.env` file in the `client` directory with the following content:

```
REACT_APP_API_URL=http://localhost:5000
```

### 3. Setting Up the Server

Navigate to the `server` directory and install the dependencies.

```bash
cd ../server
npm install
```

Create a `.env` file in the `server` directory with the following content:

```
MONGO_URI=mongodb://localhost:27017/pizaa_shop
JWT_SECRET=your_jwt_secret
PORT=5000
```

### 4. Running the Application

Start the server.

```bash
cd server
npm dev
```

In a new terminal, start the client.

```bash
cd client
npm dev
```

## Directory Structure and Key Files

### Client

- `src/`: Contains all React components and pages.
  - `components/`: Reusable UI components.
  - `pages/`: Main application pages.
  - `App.js`: Main application component.
  - `index.js`: Entry point for the React application.

### Server

- `config/`: Contains configuration files.
- `controllers/`: Contains route handlers.
- `models/`: Contains Mongoose models.
- `routes/`: Contains Express routes.
- `server.js`: Entry point for the Express server.

## Usage

### Browsing the Menu

Customers can browse the available pizzas on the main page. Each pizza displays its name, description, price, and an "Add to Cart" button.

### Placing an Order

Customers can add pizzas to their cart and proceed to checkout. At checkout, they will provide delivery information and confirm the order.

### Tracking Orders

Customers can view their order status in real-time.

### Admin Functionality

Administrators can log in to manage the menu, view orders, and update order statuses.

## Contributing

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or issues, please open an issue in the repository or contact the project maintainer at sonibk638@gmail.com
