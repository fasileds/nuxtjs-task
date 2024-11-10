<template>
  <div class="student-container">
    <!-- Title Section -->
    <div class="title-section">
      <h3>Students Also Bought</h3>
    </div>

    <!-- Course Cards List -->
    <div class="course-cards-list">
      <!-- Repeated Course Cards -->
      <div class="course-card" v-for="n in 4" :key="n">
        <div class="image-container">
          <img
            src="https://images.unsplash.com/photo-1719937050792-a6a15d899281?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
            alt="Google Cloud Certification Course"
          />
        </div>
        <div class="content-container">
          <h3 class="course-title">
            Ultimate Google Certified Cloud Architect 2024
          </h3>
          <span class="course-details">29.5 Total Hours · Updated 9/2019</span>
          <div class="rating-price">
            <span class="rating">⭐⭐⭐⭐ 4.3</span>
            <span class="students-enrolled">69,966 students</span>
            <span class="price">$19.99</span>
          </div>
        </div>
        <div class="favorite-container">
          <div class="favorite-icon">&#10084;</div>
        </div>
      </div>
    </div>
    <div class="show-more-container">Show More</div>
  </div>
</template>

<script>
export default {
  name: "StudentAlsoBought",
};
</script>

<style scoped>
.student-container {
  font-family: Arial, sans-serif;
  padding: 20px;
  max-width: 600px; /* Increased width slightly for a better display */
  margin: 0 auto;
}

.title-section h3 {
  font-size: 1.4rem;
  font-weight: bold;
  color: #2c3e50;
  margin-bottom: 15px;
}

/* Course Cards List for Vertical Layout */
.course-cards-list {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.course-card {
  display: flex;
  align-items: center;
  background-color: #f9f9f9;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  cursor: pointer;
}

.course-card:hover {
  transform: scale(1.02);
}

.image-container img {
  width: 100px;
  height: 100px;
  object-fit: cover;
  border-radius: 5px;
}

.content-container {
  flex: 1;
  margin-left: 15px;
}

.course-title {
  font-size: 1.2rem;
  font-weight: bold;
  color: #34495e;
  margin: 0;
}

.course-details {
  font-size: 0.9rem;
  color: #7f8c8d;
  margin-top: 5px;
}

.rating-price {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-top: 10px;
}

.rating {
  font-size: 1rem;
  color: #f1c40f;
}

.students-enrolled {
  font-size: 0.9rem;
  color: #95a5a6;
}

.price {
  font-size: 1rem;
  font-weight: bold;
  color: #2ecc71;
}

.favorite-container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 35px;
  height: 35px;
  border-radius: 50%;
  border: 1px solid #e74c3c;
  color: #e74c3c;
  font-size: 1.2rem;
  transition: background-color 0.3s ease;
}
.show-more-container {
  width: 100%; /* Full width */
  text-align: center;
  border: 2px solid #333; /* 2px border */
  padding: 10px;
  font-weight: bold;
  color: #333;
  cursor: pointer;
  border-radius: 5px; /* Optional rounded corners */
  transition: background-color 0.3s ease, color 0.3s ease;
}

.show-more-container:hover {
  background-color: #333;
  color: white;
}
.favorite-container:hover {
  background-color: #e74c3c;
  color: white;
}
</style>
