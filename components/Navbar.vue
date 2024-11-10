<template>
  <div class="navbar">
    <!-- Logo Section -->
    <div class="logo">
      <img
        src="https://logowik.com/content/uploads/images/udemy-new-20212512.jpg"
        alt="logo"
      />
    </div>

    <!-- Categories with Dropdown -->
    <div class="nav-item dropdown">
      <span>Categories</span>
      <div class="dropdown-content">
        <a href="#">Development</a>
        <a href="#">Business</a>
        <a href="#">Finance & Accounting</a>
        <a href="#">IT & Software</a>
        <a href="#">Personal Development</a>
      </div>
    </div>

    <!-- Search Bar with Icon -->
    <div class="search">
      <input type="text" placeholder="🔍 Search" />
    </div>

    <!-- Links with Hoverable Cards -->
    <div class="nav-item">
      <span>Udemy Business</span>
      <div class="card">
        <p>
          Get your team access to over 27,000 top Udemy courses, anytime,
          anywhere.
        </p>
        <button class="try-now-btn">Try Now</button>
      </div>
    </div>

    <div class="nav-item">
      <span>Teach on Udemy</span>
      <div class="card">
        <p>
          Turn what you know into an opportunity and reach millions around the
          world.
        </p>
        <button class="learn-more-btn">Learn More</button>
      </div>
    </div>

    <!-- Cart Icon with Hoverable Card -->
    <div class="cart">
      <span>🛒 Cart</span>
      <div class="card">
        <p>Your cart is empty.<br />Keep shopping.</p>
      </div>
    </div>

    <!-- Buttons for Authentication -->
    <div class="auth-buttons">
      <button class="login">Log In</button>
      <button class="signup">Sign Up</button>
    </div>
  </div>
</template>

<style scoped>
/* Navbar Container */
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 20px;
  background-color: #fff;
  top: 0;
  font-family: Arial, sans-serif;
}

/* Logo */
.logo img {
  width: 120px;
  cursor: pointer;
}

/* Nav Items */
.nav-item {
  font-size: 16px;
  color: #333;
  cursor: pointer;
  padding: 0 15px;
  transition: color 0.3s ease;
  position: relative;
}

.nav-item:hover {
  color: #8b25c7;
}

.dropdown-content {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background-color: #fff;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding: 10px 0;
  border-radius: 8px;
  min-width: 180px;
  z-index: 100;
}

.dropdown-content a {
  display: block;
  padding: 8px 20px;
  color: #333;
  font-size: 14px;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.dropdown-content a:hover {
  background-color: #f3eafc;
  color: #8b25c7;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.search {
  position: relative;
  z-index: 1500;
}

.search input {
  padding: 8px 35px 8px 12px;
  width: 400px;
  height: 30px;
  border-radius: 20px;
  border: 1px solid #ddd;
  transition: box-shadow 0.3s ease;
  font-size: 14px;
}

.search input::placeholder {
  color: #aaa;
}

.search input:focus {
  outline: none;
  box-shadow: 0 0 5px rgba(139, 37, 199, 0.5);
}
.card {
  display: none;
  position: absolute;
  top: 120%;
  left: 50%;
  transform: translateX(-50%);
  background-color: #ffffff;
  border: none;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.15);
  padding: 20px;
  width: 260px;
  border-radius: 12px;
  max-width: 280px;
  z-index: 1500;
  transition: opacity 0.3s ease, transform 0.3s ease;
  opacity: 0;
  transform: translate(-50%, 20px);
}

.card p {
  margin: 0;
  font-size: 15px;
  color: #333;
  line-height: 1.6;
}

.nav-item:hover .card,
.cart:hover .card {
  display: block;
  opacity: 1;
  transform: translate(-50%, 0);
}
.try-now-btn,
.learn-more-btn {
  display: inline-block;
  margin-top: 12px;
  padding: 8px 16px;
  font-size: 14px;
  font-weight: bold;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.try-now-btn {
  background-color: #8b25c7;
  color: #fff;
}

.try-now-btn:hover {
  background-color: #a73fe6;
  transform: scale(1.05);
}

.learn-more-btn {
  background-color: #f4f4f6;
  color: #333;
  border: 1px solid #ddd;
}

.learn-more-btn:hover {
  background-color: #e6e6e8;
  transform: scale(1.05);
}

/* Cart */
.cart {
  font-size: 16px;
  cursor: pointer;
  color: #333;
  position: relative;
}

.cart:hover {
  color: #8b25c7;
}
.auth-buttons .login,
.auth-buttons .signup {
  padding: 8px 16px;
  font-size: 14px;
  cursor: pointer;
  border: none;
  transition: background-color 0.3s ease;
}

.auth-buttons .login {
  background-color: #fff;
  color: #8b25c7;
  border: 1px solid #8b25c7;
  margin-right: 10px;
}

.auth-buttons .login:hover {
  background-color: #f3eafc;
}

.auth-buttons .signup {
  background-color: #8b25c7;
  color: #fff;
}

.auth-buttons .signup:hover {
  background-color: #6f1d9f;
}

.card {
  animation: fadeInUp 0.4s ease forwards;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
