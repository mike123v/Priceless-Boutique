body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
  }
  
  header {
    background-color: #333;
    color: white;
    padding: 40px 20px;
    text-align: center;
  }
  
  .search-container {
    text-align: center;
    margin: 20px;
  }
  
  #searchBar {
    width: 80%;
    max-width: 400px;
    padding: 10px;
    font-size: 16px;
  }
  
  .filter-buttons {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .filter-buttons button {
    padding: 10px 15px;
    margin: 5px;
    background-color: #555;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .filter-buttons button:hover {
    background-color: #333;
  }
  
  .products {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
  }
  
  .product {
    background-color: white;
    border: 1px solid #ddd;
    border-radius: 10px;
    margin: 10px;
    padding: 20px;
    width: 250px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  }
  
  .product img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 8px;
  }
  
  .buy-btn {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 15px;
    background-color: #25D366;
    color: white;
    text-decoration: none;
    border-radius: 5px;
  }
  
  footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: white;
  }
  
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Product Store</title>
  <link rel="stylesheet" href="B.CSS" />
</head>
<body>
  <header>
    <h1>Welcome to Priceless Boutique</h1>
    <p>Browse products and contact me to make a deal!</p>
  </header>

  <!-- Search Bar -->
  <div class="search-container">
    <input type="text" id="searchBar" placeholder="Search for a product..." onkeyup="searchProducts()" />
  </div>

  <!-- Category Filter Buttons -->
  <div class="filter-buttons">
    <button onclick="filterProducts('all')">All</button>
 <button onclick="filterProducts('accessories')">Accessories</button>
    <button onclick="filterProducts('Watches&Jewelry')">Watches&Jewelry</button>
  </div>

  <!-- Product List -->

      <!-- Product 1 -->
  <section class="products">
    <div class="product" data-category="Watches&Jewelry">
        <img src="c:\Users\M charlene\Pictures\Camera Roll\IMG_4980.jpeg.jpg" alt="New 2023 Business Watch Men's quartz watch Sporty wind trend Leisure Men's bracelet set Europe and America" />
        <h2>New 2023 Business Watch Men's quartz watch Sporty wind trend Leisure Men's bracelet set Europe and America</h2>
        <p>7,782~9,091 RWF
        </p>
        <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
      </div>
  
      <!-- Product 2 -->
      <section class="products">
        <div class="product" data-category="Watches&Jewelry">
            <img src="c:\Users\M charlene\Pictures\Camera Roll\IMG_4977.jpeg.jpg" alt="jewelry" />
            <h2>
                Fashion crystal sequin necklace temperament trend multi-layer metal pendant clavicle chain jewelry</h2>
            <p>3,366 RWF</p>
            <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
          </div>
      
            <!-- Product 3 -->

            <section class="products">
                <div class="product" data-category="Watches&Jewelry">
                    <img src="c:\Users\M charlene\Pictures\Camera Roll\IMG_4952.jpeg.jpg" alt="jewelry" />
                    <h2>6PCS Set Luxury Watch Women Ring Necklace Earring Rhinestone Fashion Wristwatch Casual Ladies Watches Bracelet Set Clock
                        </h2>
                    <p>16000RWF</p>
                    <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
                  </div>
            
                    <!-- Product 4 -->
                    <section class="products">
                        <div class="product" data-category="Watches&Jewelry">
                            <img src="c:\Users\M charlene\Pictures\Camera Roll\IMG_4960.jpeg.jpg" alt="Watch" />
                            <h2>New Digital LED Watch For Men Multifunction Alarm Electronic Clock Waterproof Simple Men Women Stopwatch LED Watches Clocks
                                </h2>
                            <p>15000RWF</p>
                            <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
                          </div>
                   
                    <!-- Product 5 -->
                    <section class="products">
                        <div class="product" data-category="Watches&Jewelry">
                            <img src="c:\Users\M charlene\Pictures\Camera Roll\IMG_4955.jpeg.jpg" alt="Rings" />
                            <h2>New open multi-joint ring set 22-piece love ring female design sense niche butterfly ring jewelry
                                </h2>
                            <p>15000RWF</p>
                            <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
                          </div>
                    
                    <!-- Product 6 -->
<section class="products">
    <div class="product" data-category="Watches&Jewelry">
        <img src="c:\Users\M charlene\Pictures\Camera Roll\IMG_4982.jpeg.jpg" alt="chain" />
        <h2>Fashion personality leaf pearl water drop clavicle chain
            </h2>
        <p>15000RWF</p>
        <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
      </div>
</section>


                    

    <!-- Product 2 -->

    <div class="product" data-category="accessories">
      <img src="hat.jpg" alt="Fashion Hat" />
      <h2>Fashion Hat</h2>
      <p>$15.00</p>
      <a href="https://wa.me/+250791811619" target="_blank" class="buy-btn">Contact to Buy</a>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 My Store. All rights reserved.</p>
  </footer>

  <!-- Scripts -->
  <script>
    function searchProducts() {
      const input = document.getElementById("searchBar").value.toLowerCase();
      const products = document.getElementsByClassName("product");

      for (let i = 0; i < products.length; i++) {
        const name = products[i].getElementsByTagName("h2")[0].textContent.toLowerCase();
        products[i].style.display = name.includes(input) ? "" : "none";
      }
    }

    function filterProducts(category) {
      const products = document.querySelectorAll('.product');

      products.forEach(product => {
        const productCategory = product.getAttribute('data-category');

        if (category === 'all' || productCategory === category) {
          product.style.display = 'block';
        } else {
          product.style.display = 'none';
        }
      });
    }
  </script>
</body>
</html>

