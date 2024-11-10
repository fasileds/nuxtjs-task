<template>
  <div class="course-header">
    <h3>
      More Courses by
      <span class="course-provider">TechLink Selenium | DevOps | GenAI</span>
    </h3>
  </div>
  <div class="course-cards-container">
    <div class="course-card">
      <div class="course-image">
        <img
          src="https://images.unsplash.com/photo-1521566652839-697aa473761a?q=80&w=1471&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Course Image"
        />
      </div>

      <div class="course-details">
        <span class="course-title"
          >DevOps MasterClass 2024: Terraform Kubernetes ...</span
        >
        <span class="course-provider-info"
          >TechLink Selenium | DevOps | GenAI</span
        >
        <span class="course-rating">
          <i class="fas fa-star"></i> 4.5 <span>(6,311)</span>
        </span>

        <div class="course-meta">
          <ul>
            <li><i class="fas fa-clock"></i> 76.5 Total Hours</li>
            <li><i class="fas fa-chalkboard-teacher"></i> 548 Lectures</li>
            <li><i class="fas fa-level-up-alt"></i> All Levels</li>
          </ul>
        </div>

        <span class="course-price">$69.99</span>
      </div>
    </div>

    <!-- Duplicate the card for additional courses -->
    <div class="course-card">
      <div class="course-image">
        <img
          src="https://images.unsplash.com/photo-1521566652839-697aa473761a?q=80&w=1471&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Course Image"
        />
      </div>

      <div class="course-details">
        <span class="course-title"
          >DevOps MasterClass 2024: Terraform Kubernetes ...</span
        >
        <span class="course-provider-info"
          >TechLink Selenium | DevOps | GenAI</span
        >
        <span class="course-rating">
          <i class="fas fa-star"></i> 4.5 <span>(6,311)</span>
        </span>

        <div class="course-meta">
          <ul>
            <li><i class="fas fa-clock"></i> 76.5 Total Hours</li>
            <li><i class="fas fa-chalkboard-teacher"></i> 548 Lectures</li>
            <li><i class="fas fa-level-up-alt"></i> All Levels</li>
          </ul>
        </div>

        <span class="course-price">$69.99</span>
      </div>
    </div>

    <div class="course-card">
      <div class="course-image">
        <img
          src="https://images.unsplash.com/photo-1521566652839-697aa473761a?q=80&w=1471&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
          alt="Course Image"
        />
      </div>

      <div class="course-details">
        <span class="course-title"
          >DevOps MasterClass 2024: Terraform Kubernetes ...</span
        >
        <span class="course-provider-info"
          >TechLink Selenium | DevOps | GenAI</span
        >
        <span class="course-rating">
          <i class="fas fa-star"></i> 4.5 <span>(6,311)</span>
        </span>

        <div class="course-meta">
          <ul>
            <li><i class="fas fa-clock"></i> 76.5 Total Hours</li>
            <li><i class="fas fa-chalkboard-teacher"></i> 548 Lectures</li>
            <li><i class="fas fa-level-up-alt"></i> All Levels</li>
          </ul>
        </div>

        <span class="course-price">$69.99</span>
      </div>
    </div>
  </div>
  <div class="report-abuse">
    <span>Report abuse</span>
  </div>
</template>

<script>
// Add any logic if needed
</script>

<style scoped>
/* Container for the cards */
.course-header h3 {
  font-size: 1.5rem;
  color: #333;
  margin-bottom: 15px;
}

.course-provider {
  font-weight: bold;
  color: #db34db;
}
.course-cards-container {
  display: flex;
  padding: 20px;
}

/* Styling for each individual course card */
.course-card {
  background-color: white;
  width: 30%;
  overflow: hidden;
  padding: 15px;
  transition: transform 0.3s ease;
}

.course-card:hover {
  transform: translateY(-5px);
}

/* Course image */
.course-image img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

/* Course details section */
.course-details {
  margin-top: 15px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}

/* Title and general text styles */
.course-title {
  font-size: 1.3rem;
  font-weight: bold;
  color: #2c3e50;
}

.course-provider-info {
  color: #7f8c8d;
  font-size: 1rem;
}

/* Rating */
.course-rating {
  font-size: 1rem;
  color: #f39c12;
  display: flex;
  align-items: center;
}

.course-rating .fas {
  color: #f39c12;
  margin-right: 5px;
}

/* Horizontally aligned list */
.course-meta ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  display: flex;
  gap: 20px;
}

.course-meta li {
  font-size: 0.9rem;
  color: #2c3e50;
  display: flex;
  align-items: center;
  gap: 10px;

  font-size: 9px;
}

.course-meta li i {
  color: #16a085;
}
.course-price {
  font-size: 1.4rem;
  font-weight: bold;
  color: #27ae60;
  margin-top: 10px;
}
.report-abuse {
  width: 100%;
  text-align: center;
  border: 1px solid #333;
  padding: 10px;
  font-weight: bold;
  color: #333;
  cursor: pointer;
  transition: background-color 0.3s ease, color 0.3s ease;
}

.report-abuse span {
  font-size: 1.2rem;
  font-weight: bold;
  cursor: pointer;
}

.report-abuse:hover {
  background-color: #d8d8d8;
}
</style>
