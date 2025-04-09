# my-website
New e-commerce Website 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>ElectroStore - Electrical Goods</title>
  <!-- Importing Google Fonts for a modern sans-serif look -->
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* Base Styles */
    body {
      margin: 0;
      font-family: 'Roboto', sans-serif;
      background-color: #ECF0F1; /* Soft Light Gray */
      color: #2C3E50; /* Dark Gray / Near-Black */
    }
    
    /* Header Styles */
    .header {
      background-color: #2C3E50; /* Navy/Slate Blue */
      color: #fff;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .header .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }
    .header .nav-icons {
      display: flex;
      gap: 15px;
    }
    .header .nav-icons i {
      font-size: 1.5rem;
      cursor: pointer;
      color: #3498DB; /* Electric Blue for interactive icons */
    }
    
    /* Banner Styles */
    .banner {
      background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(44, 62, 80, 0.8)),
                  url('placeholder-banner-image.jpg') no-repeat center center;
      background-size: cover;
      color: #FFF;
      text-align: center;
      padding: 50px 20px;
    }
    .banner h1 {
      margin: 0 0 10px;
      font-size: 2rem;
    }
    .banner p {
      margin: 0 0 20px;
    }
    .btn-primary {
      background-color: #3498DB;
      color: #fff;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 5px;
      transition: background-color 0.3s;
    }
    .btn-primary:hover {
      background-color: #1ABC9C; /* Turquoise Accent */
    }
    
    /* Editable Text Box (for promotional text, etc.) */
    .editable-text {
      border: 1px dashed #3498DB;
      margin: 20px auto 0;
      max-width: 90%;
      padding: 10px;
      color: #FFFFFF;
      background: rgba(0,0,0,0.3);
    }
    
    /* Product List Styles */
    .products {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      padding: 20px;
    }
    .product {
      background-color: #fff;
      border: 1px solid #ddd;
      border-radius: 8px;
      margin: 10px;
      width: calc(100%/2 - 40px);
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      display: flex;
      flex-direction: column;
      transition: transform 0.3s;
    }
    .product:hover {
      transform: translateY(-5px);
    }
    .product img {
      width: 100%;
      border-top-left-radius: 8px;
      border-top-right-radius: 8px;
    }
    .product-details {
      padding: 15px;
      flex-grow: 1;
    }
    .product-details h3 {
      margin: 0 0 10px;
      font-size: 1.2rem;
    }
    .product-details p {
      margin: 0 0 10px;
      font-size: 1rem;
    }
    .product-details .price {
      font-weight: bold;
      margin-bottom: 10px;
    }
    .product-buttons {
      display: flex;
      justify-content: space-between;
      padding: 0 15px 15px;
    }
    .btn {
      background-color: #3498DB;
      color: #fff;
      border: none;
      padding: 8px 10px;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s;
      font-size: 0.9rem;
    }
    .btn:hover {
      background-color: #1ABC9C;
    }
    
    /* Footer Styles */
    .footer {
      background-color: #2C3E50;
      color: #FFF;
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
    }
    
    /* Responsive Adjustments */
    @media (min-width: 600px) {
      .product {
        width: calc(100%/3 - 40px);
      }
    }
    @media (min-width: 1024px) {
      .product {
        width: calc(100%/4 - 40px);
      }
    }
  </style>
</head>
<body>
  
  <!-- Header Section -->
  <header class="header">
    <div class="logo">ElectroStore</div>
    <div class="nav-icons">
      <!-- Replace icons with proper links or use JavaScript for actions -->
      <i class="fas fa-search"></i>
      <i class="fas fa-shopping-cart"></i>
      <i class="fas fa-bars"></i>
    </div>
  </header>
  
  <!-- Banner Section -->
  <section class="banner">
    <h1 contenteditable="true">Welcome to ElectroStore</h1>
    <p contenteditable="true">Discover the latest in electrical goods and accessories</p>
    <a class="btn-primary" href="#">Shop Now</a>
    <!-- An editable text box for additional promotional info -->
    <div class="editable-text" contenteditable="true">
      Edit this text to add promotional info.
    </div>
  </section>
  
  <!-- Product Listing Section -->
  <section class="products">
    <!-- Example Product Card 1 -->
    <div class="product">
      <img src="placeholder-product1.jpg" alt="Product 1">
      <div class="product-details">
        <h3 contenteditable="true">Product Title 1</h3>
        <p contenteditable="true">Short product description goes here. Click to edit this content.</p>
        <div class="price">$99.99</div>
      </div>
      <div class="product-buttons">
        <button class="btn">Add to Cart</button>
        <button class="btn">Edit</button>
      </div>
    </div>
    
    <!-- Example Product Card 2 -->
    <div class="product">
      <img src="placeholder-product2.jpg" alt="Product 2">
      <div class="product-details">
        <h3 contenteditable="true">Product Title 2</h3>
        <p contenteditable="true">Short product description goes here. Click to edit this content.</p>
        <div class="price">$149.99</div>
      </div>
      <div class="product-buttons">
        <button class="btn">Add to Cart</button>
        <button class="btn">Edit</button>
      </div>
    </div>
    
    <!-- Additional product cards can be added here as needed -->
  </section>
  
  <!-- Footer Section -->
  <footer class="footer">
    &copy; 2025 ElectroStore. All rights reserved.
  </footer>
  
  <!-- Adding Font Awesome for icons (ensure you have internet connectivity or host locally) -->
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
