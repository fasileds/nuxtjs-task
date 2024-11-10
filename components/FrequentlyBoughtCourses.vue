<template>
  <div class="frequently-bought-container">
    <!-- Header -->
    <div class="header">
      <h2>Frequently Bought Together</h2>
    </div>

    <!-- Product Card -->
    <div class="product-card">
      <div class="product-image">
        <img
          src="https://images.unsplash.com/photo-1719937050792-a6a15d899281?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Product Image"
        />
      </div>
      <div class="product-details">
        <h3>Google Cloud Professional Cloud Architect: GCP Certification</h3>
        <span class="instructor">TechLink Silanium | DevOps | GenAI</span>
        <span class="rating">⭐⭐⭐⭐ 4.3 <span>(431)</span></span>
        <div class="best-seller">Best Seller</div>
      </div>
      <div class="price">$49.99</div>
    </div>
    <div class="product-card">
      <div class="product-image">
        <img
          src="https://images.unsplash.com/photo-1719937050792-a6a15d899281?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Product Image"
        />
      </div>
      <div class="product-details">
        <h3>Google Cloud Professional Cloud Architect: GCP Certification</h3>
        <span class="instructor">TechLink Silanium | DevOps | GenAI</span>
        <span class="rating">⭐⭐⭐⭐ 4.3 <span>(431)</span></span>
        <div class="best-seller">Best Seller</div>
      </div>
      <div class="price">$49.99</div>
    </div>
    <div class="product-card">
      <div class="product-image">
        <img
          src="https://images.unsplash.com/photo-1719937050792-a6a15d899281?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Product Image"
        />
      </div>
      <div class="product-details">
        <h3>Google Cloud Professional Cloud Architect: GCP Certification</h3>
        <span class="instructor">TechLink Silanium | DevOps | GenAI</span>
        <span class="rating">⭐⭐⭐⭐ 4.3 <span>(431)</span></span>
        <div class="best-seller">Best Seller</div>
      </div>
      <div class="price">$49.99</div>
    </div>
    <div class="product-card">
      <div class="product-image">
        <img
          src="https://images.unsplash.com/photo-1719937050792-a6a15d899281?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Product Image"
        />
      </div>
      <div class="product-details">
        <h3>Google Cloud Professional Cloud Architect: GCP Certification</h3>
        <span class="instructor">TechLink Silanium | DevOps | GenAI</span>
        <span class="rating">⭐⭐⭐⭐ 4.3 <span>(431)</span></span>
        <div class="best-seller">Best Seller</div>
      </div>
      <div class="price">$49.99</div>
    </div>

    <div class="total-section">
      <span class="total-label"
        >Total: <span class="total-price">$144.97</span></span
      >
      <button class="add-to-cart-btn">Add All To Cart</button>
    </div>
  </div>
</template>

<style scoped>
.frequently-bought-container {
  font-family: Arial, sans-serif;
  background-color: #f9f9f9;
  padding: 30px;
  border: 1px solid rgb(122, 122, 122);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
  max-width: 800px;
  margin: 30px auto;
}

.header h2 {
  font-size: 1.75rem;
  color: #333;
  margin-bottom: 25px;
  text-align: center;
}

.product-card {
  display: flex;
  align-items: center;
  padding: 20px;
  border-radius: 10px;
  background-color: white;
  margin-bottom: 20px;
  transition: transform 0.3s;
  box-shadow: 0 3px 8px rgba(0, 0, 0, 0.1);
}

.product-card:hover {
  transform: scale(1.03);
}

.product-image img {
  width: 120px;
  height: 120px;
  border-radius: 8px;
  object-fit: cover;
  margin-right: 20px;
}

.product-details {
  flex-grow: 1;
}

.product-details h3 {
  font-size: 1.2rem;
  color: #333;
  margin: 0;
  line-height: 1.4;
}

.instructor {
  display: block;
  font-size: 0.9rem;
  color: #666;
  margin-top: 5px;
}

.rating {
  color: #ffa500;
  font-size: 1rem;
  margin-top: 10px;
  display: inline-block;
}

.best-seller {
  background-color: #ff6f61;
  color: white;
  font-size: 0.8rem;
  padding: 4px 10px;
  border-radius: 5px;
  margin-top: 8px;
  display: inline-block;
}

.price {
  font-size: 1.3rem;
  font-weight: bold;
  color: #333;
  margin-left: 20px;
}

.total-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 25px;
  padding-top: 10px;
  border-top: 2px solid #e0e0e0;
}

.total-label {
  font-size: 1.1rem;
  color: #333;
}

.total-price {
  font-weight: bold;
  font-size: 1.3rem;
  color: #333;
}

.add-to-cart-btn {
  padding: 12px 25px;
  background-color: #ac2eb3;
  color: white;
  border: none;
  font-weight: bold;
  height: 50px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.add-to-cart-btn:hover {
  background-color: #c94acf;
}
</style>
