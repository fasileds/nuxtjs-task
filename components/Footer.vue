<template>
  <div class="footer-container">
    <div class="footer-top">
      <div class="footer-description">
        <span>
          Top companies choose Udemy Business to build in-demand career skills.
        </span>
      </div>
      <div class="footer-images">
        <img
          src="/images-removebg-preview.png"
          alt="Company Image 1"
          class="footer-image"
        />
        <img
          src="/images-removebg-preview.png"
          alt="Company Image 2"
          class="footer-image"
        />
        <img
          src="/images-removebg-preview.png"
          alt="Company Image 3"
          class="footer-image"
        />
        <img
          src="/images-removebg-preview.png"
          alt="Company Image 4"
          class="footer-image"
        />
      </div>
    </div>

    <div class="footer-links">
      <div class="footer-column">
        <ul>
          <li><a href="#">Udemy Business</a></li>
          <li><a href="#">Teach on Udemy</a></li>
          <li><a href="#">Get the app</a></li>
          <li><a href="#">About us</a></li>
          <li><a href="#">Contact us</a></li>
        </ul>
      </div>
      <div class="footer-column">
        <ul>
          <li><a href="#">Careers</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Help and Support</a></li>
          <li><a href="#">Affiliate</a></li>
          <li><a href="#">Investors</a></li>
        </ul>
      </div>
      <div class="footer-column">
        <ul>
          <li><a href="#">Terms</a></li>
          <li><a href="#">Privacy policy</a></li>
          <li><a href="#">Cookie Settings</a></li>
          <li><a href="#">Sitemap</a></li>
          <li><a href="#">Accessibility statement</a></li>
        </ul>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="language-selector">
        <span>English</span>
      </div>
      <div class="footer-info">
        <img
          src="/OIP-removebg-preview.png"
          alt="Udemy Logo"
          class="footer-logo"
        />
        <span>© 2024 Udemy, Inc</span>
      </div>
    </div>
  </div>
</template>

<script>
// Add any necessary JavaScript or logic here
</script>

<style scoped>
/* Overall Footer Container */
.footer-container {
  background-color: #2b2f31;
  padding: 40px 20px;
  font-family: "Arial", sans-serif;
  color: white;
}

/* Top Section */
.footer-top {
  margin-bottom: 40px;
}

.footer-description {
  font-size: 1.3rem;
  font-weight: bold;
  text-align: center;
  margin-bottom: 20px;
}

.footer-images {
  display: flex;
  justify-content: space-around;
  gap: 10px;
}

.footer-image {
  max-width: 150px;
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 10px;
  transition: transform 0.3s ease;
}

.footer-image:hover {
  transform: scale(1.1);
}

/* Footer Links Section */
.footer-links {
  display: flex;
  justify-content: space-around;
  margin-bottom: 40px;
}

.footer-column ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

.footer-column li {
  margin-bottom: 10px;
}

.footer-column a {
  text-decoration: none;
  color: #f1f1f1;
  font-size: 1rem;
  transition: color 0.3s ease;
}

.footer-column a:hover {
  color: #ff9800;
}

/* Footer Bottom Section */
.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 0.9rem;
}

.language-selector {
  padding: 8px 15px;
  border: 2px solid #fff;
  border-radius: 5px;
  color: white;
  font-size: 1rem;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
}

.language-selector:hover {
  background-color: #ff9800;
  border-color: #ff9800;
}

.footer-info {
  display: flex;
  align-items: center;
  gap: 15px;
}

.footer-logo {
  max-width: 100px;
  height: auto;
}

.footer-info span {
  font-size: 1rem;
  color: #f1f1f1;
}
</style>
