<template>
  <div class="container">
    <div class="left-side">
      <span class="category">
        Development > Software Engineering > Google Cloud Professional Cloud
        Architect
      </span>
      <h1 class="course-title">
        Google Cloud Professional Cloud Architect: GCP Certification
      </h1>
      <h3 class="course-description">
        Google Cloud Professional Cloud Architect Certification. Become a GCP
        Cloud Architect, Latest GCP Exam and Case Studies.
      </h3>
      <div class="course-details">
        <div class="best-seller">Best seller</div>
        <div class="rating">
          <span class="rating-text">4.4</span>
          <span class="star-icon">
            ⭐⭐⭐⭐
            <!-- Empty star -->
          </span>
          <span class="ratings-info">(431 ratings)</span>
          <span class="students-count">17,694 students</span>
        </div>
      </div>
      <div class="creator-info">
        <span>
          Created By
          <span class="creator-name">Tech Link Sileniyume</span>
        </span>
        <span class="updated-info">Last updated 4/2023</span>
        <span class="language-info">
          <i class="fas fa-language"></i> English
        </span>
      </div>
    </div>
    <div class="right-side">
      <!-- You can add additional content or images here if needed -->
    </div>
  </div>
</template>

<script>
export default {
  name: "CourseDetails",
};
</script>

<style scoped>
/* General container setup */
.container {
  display: flex;
  background-color: #1f1f1f; /* Dark background to match the navbar */
  padding: 30px;
  color: white;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transition: all 0.3s ease;
}

.container:hover {
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
}

/* Left-side styling */
.left-side {
  flex: 2;
  padding: 20px;
  font-family: "Arial", sans-serif;
}

/* Right-side styling */
.right-side {
  flex: 1;
}

/* Category text */
.category {
  font-size: 14px;
  font-weight: bold;
  color: #8072e6; /* Lighter, softer purple */
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* Course title */
.course-title {
  font-size: 32px;
  font-weight: bold;
  margin-top: 10px;
  color: #fff;
  transition: color 0.3s ease;
}

.course-title:hover {
  color: #8072e6; /* Lighter purple on hover */
}

/* Course description */
.course-description {
  font-size: 18px;
  color: #ddd;
  margin-top: 10px;
}

/* Course details layout */
.course-details {
  display: flex;
  gap: 20px;
  align-items: center;
  margin-top: 20px;
}

/* Best-seller badge */
.best-seller {
  background-color: #f0edbc;
  padding: 8px 12px;
  font-size: 16px;
  font-weight: bold;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  color: #333; /* Light black text color */
  transition: background-color 0.3s ease, transform 0.3s ease;
}

.best-seller:hover {
  background-color: #e3d79b; /* Lighter yellow */
  transform: translateY(-3px);
}

.rating {
  display: flex;
  align-items: center;
  font-size: 18px;
}

.star-icon i {
  color: #8072e6; /* Lighter purple */
  margin-right: 5px;
  transition: transform 0.3s ease;
}

.star-icon i:hover {
  transform: scale(1.2);
}

.rating-text {
  font-size: 22px;
  font-weight: bold;
  margin-right: 10px;
}

.ratings-info {
  font-size: 16px;
  color: #ccc;
  margin-left: 5px;
}

.students-count {
  font-size: 16px;
  color: #ccc;
  margin-left: 10px;
}

.creator-info {
  margin-top: 30px;
}

.creator-name {
  font-weight: bold;
  color: #8072e6; /* Lighter purple */
  transition: color 0.3s ease;
}

.creator-name:hover {
  color: #6c4ecf; /* Slightly deeper purple on hover */
}

.updated-info {
  display: block;
  margin-top: 5px;
  font-size: 14px;
  color: #888;
}

.language-info {
  display: block;
  margin-top: 5px;
  font-size: 16px;
  color: #888;
}

.language-info i {
  margin-right: 5px;
  color: #8072e6; /* Lighter purple */
  transition: color 0.3s ease;
}

.language-info i:hover {
  color: #6c4ecf; /* Slightly deeper purple on hover */
}
</style>
