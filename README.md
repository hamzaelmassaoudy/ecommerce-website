<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PHP MySQL Online Marketplace</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      margin: 20px;
    }
    h1, h2, h3 {
      color: #333;
    }
    ul {
      list-style-type: disc;
      margin-left: 20px;
    }
    pre {
      background-color: #f4f4f4;
      padding: 10px;
      border-radius: 5px;
      overflow-x: auto;
    }
    a {
      color: #007BFF;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .banner {
      text-align: center;
      margin-bottom: 20px;
    }
    .banner img {
      max-width: 100%;
      height: auto;
    }
  </style>
</head>
<body>

  <div class="banner">
    <img src="link_to_banner_image" alt="Marketplace Banner">
  </div>

  <h1>🛒 PHP MySQL Online Marketplace</h1>

  <p>This project is an <strong>online marketplace platform</strong> developed using <strong>PHP for server-side scripting</strong> and <strong>MySQL for database management</strong>. It allows users to seamlessly <strong>buy and sell products</strong> in a user-friendly environment. The platform demonstrates the integration of backend logic with a relational database to create a fully functional e-commerce system.</p>

  <h2>🎯 Key Features</h2>
  <ul>
    <li>🔐 User Authentication – Users can register, log in, and manage their profiles securely</li>
    <li>🛍 Product Management – Sellers can add, edit, and delete product listings with descriptions, prices, and images</li>
    <li>🔎 Advanced Search & Filters – Users can search for products and refine results using filters</li>
    <li>🛒 Shopping Cart System – Add products to your cart and complete purchases effortlessly</li>
    <li>📦 Order Tracking – Admins and sellers can manage orders, update statuses, and track deliveries</li>
  </ul>

  <h2>🔑 Login Credentials</h2>
  <ul>
    <li><strong>🖥 Admin Login:</strong> <code>iqbolshoh</code></li>
    <li><strong>👤 Seller Login:</strong> <code>user</code></li>
    <li><strong>👤 Customer Login:</strong> <code>user</code></li>
    <li><strong>🔑 Password:</strong> <code>IQBOLSHOH</code></li>
  </ul>

  <h2>👥 User Roles and Permissions</h2>
  <h3>🏆 Admin</h3>
  <ul>
    <li>Full control over the marketplace</li>
    <li>Manage users, products, and orders</li>
    <li>Approve or reject product listings</li>
    <li>Resolve disputes and update order statuses</li>
    <li>Block or deactivate user accounts</li>
  </ul>

  <h3>🛒 Seller</h3>
  <ul>
    <li>Add, edit, and delete product listings</li>
    <li>View and manage orders placed for their products</li>
    <li>Update inventory and product details</li>
    <li>Track sales performance</li>
  </ul>

  <h3>👤 Customer</h3>
  <ul>
    <li>Browse and search for products</li>
    <li>Add products to the shopping cart and checkout</li>
    <li>View order history and track deliveries</li>
    <li>Manage personal profile and payment information</li>
  </ul>

  <h2>🛠 Setup Instructions</h2>
  <h3>1️⃣ Prerequisites</h3>
  <ul>
    <li>Install a <strong>PHP-compatible server</strong> (e.g., XAMPP, WAMP, or LAMP).</li>
    <li>Install <strong>MySQL</strong> for database management.</li>
  </ul>

  <h3>2️⃣ Set Up the Database</h3>
  <pre>
CREATE DATABASE marketplace;

mysql -u yourusername -p marketplace < db/schema.sql
  </pre>

  <h3>3️⃣ Configure Database Connection</h3>
  <pre>
<?php

class Database {
    private $conn;

    public function __construct() {
        $servername = "localhost";
        $username = "your_username";
        $password = "your_password";
        $dbname = "marketplace";

        $this->conn = new mysqli($servername, $username, $password, $dbname);

        if ($this->conn->connect_error) {
            die("Connection failed: " . $this->conn->connect_error);
        }
    }

    public function getConnection() {
        return $this->conn;
    }
}
?>
  </pre>

  <h3>4️⃣ Run the Application</h3>
  <ol>
    <li>Deploy the project on your local server (e.g., Apache or Nginx).</li>
    <li>Access the application via your browser:</li>
    <pre>http://localhost/php-mysql-marketplace</pre>
  </ol>

  <h2>🌟 Future Enhancements</h2>
  <ul>
    <li>Payment Gateway Integration – Add support for PayPal, Stripe, or other payment processors</li>
    <li>Responsive Design – Optimize the UI for mobile and tablet devices</li>
    <li>Email Notifications – Notify users about order updates and promotions</li>
    <li>Wishlist Feature – Allow users to save products for later purchase</li>
    <li>Advanced Analytics – Provide sellers with detailed sales reports and insights</li>
  </ul>

  <p>This <strong>PHP MySQL Marketplace</strong> project is a great starting point for building a scalable e-commerce platform. Customize it further to suit your specific requirements and take your online store to the next level!</p>

  <p>🎉 <strong>Happy Coding!</strong> 🎉</p>

</body>
</html>