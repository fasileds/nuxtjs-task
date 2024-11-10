<template>
  <div class="course-content">
    <!-- Learning Section -->
    <section class="learning-section">
      <h1 class="section-title">What you'll learn</h1>
      <div class="learning-lists">
        <ul class="learning-list left">
          <li>
            Start your journey to become a Google Cloud Certified Professional
            Cloud Architect
          </li>
          <li>
            Students will learn about data storage options like Persistent disk,
            Local Disk, Cloud SQL, Cloud DataStore, BigQuery
          </li>
          <li>
            Understand the best practices for building available, scalable,
            resilient, and secure applications on the Google Cloud Platform
          </li>
        </ul>
        <ul class="learning-list right">
          <li>
            Get hands-on with compute, networking, storage, and database
            services in Google Cloud Platform
          </li>
          <li>
            Understand how to architect and deploy secure and robust
            applications on Google Cloud Platform
          </li>
        </ul>
      </div>
    </section>

    <!-- Course Includes Section -->
    <section class="course-includes">
      <h1 class="section-title">This course includes:</h1>
      <div class="includes-lists">
        <ul class="includes-list left">
          <li>22 hours on-demand video</li>
          <li>16 articles</li>
          <li>81 downloadable resources</li>
        </ul>
        <ul class="includes-list right">
          <li>Access on mobile and TV</li>
          <li>Certificate of completion</li>
        </ul>
      </div>
    </section>

    <!-- Companies Offer Section -->
    <section class="companies-offer">
      <h3 class="section-title">
        Top companies offer this course to their employees
      </h3>
      <p class="description">
        This course was selected for our collection of top-rated courses trusted
        by businesses worldwide.
        <span class="learn-more">Learn more</span>
      </p>
      <ul class="companies-logos">
        <li>
          <img
            src="/images-removebg-preview.png"
            alt="Company Logo"
            class="company-logo"
          />
        </li>
        <li>
          <img
            src="/images-removebg-preview.png"
            alt="Company Logo"
            class="company-logo"
          />
        </li>
        <li>
          <img
            src="/images-removebg-preview.png"
            alt="Company Logo"
            class="company-logo"
          />
        </li>
        <li>
          <img
            src="/images-removebg-preview.png"
            alt="Company Logo"
            class="company-logo"
          />
        </li>
        <!-- You can add more logos here -->
      </ul>
    </section>
  </div>
</template>

<script setup></script>

<style scoped>
/* General Styles */
.course-content {
  max-width: 1200px;
  margin: 0 auto;
  padding: 40px;
  background-color: white;
}

/* Section Title Styles */
.section-title {
  font-size: 28px;
  font-weight: bold;
  color: #333;
  margin-bottom: 20px;
}

/* Learning Section Styles */
.learning-section {
  border: 1px solid #ddd; /* Light gray border */
  background-color: #f0efef;
  padding: 20px;
  margin-bottom: 30px;
}

.learning-lists {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.learning-list {
  list-style: none;
  padding-left: 0;
  font-size: 14px;
  color: #555;
}

.learning-list li {
  margin-bottom: 15px;
  line-height: 1.6;
}

.learning-list li::before {
  content: "✔";
  margin-right: 10px;
  color: #5022c3; /* Purple color */
}

/* Course Includes Section */
.course-includes {
  background-color: #fff;
  border-radius: 8px;
  padding: 20px;
  margin-bottom: 30px;
}

.includes-lists {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.includes-list {
  list-style: none;
  padding-left: 0;
  font-size: 14px; /* Decreased font size */
  color: #555;
}

.includes-list li {
  margin-bottom: 15px;
  line-height: 1.6;
}

.includes-list li::before {
  content: "✔";
  margin-right: 10px;
  color: #5022c3; /* Purple color */
}

/* List Styles for Left and Right Sections */
.left {
  flex: 1;
}

.right {
  flex: 1;
}

.companies-offer {
  border: 1px solid #ddd;
  background-color: #e4e1e1;
  padding: 30px;
}
.companies-offer .description {
  font-size: 16px;
  color: #555;
  margin-bottom: 20px;
}

.learn-more {
  color: #5022c3;
  cursor: pointer;
  font-weight: bold;
}

.learn-more:hover {
  text-decoration: underline;
}

.companies-logos {
  display: flex;
  list-style: none;

  gap: 40px;
  justify-content: flex-start;
}

.company-logo {
  height: 50px;
  width: 90px;
  object-fit: contain;
}

/* Media Queries for Responsiveness */
@media (max-width: 768px) {
  .course-content {
    padding: 20px;
  }

  .section-title {
    font-size: 24px;
  }

  .learning-list li,
  .includes-list li {
    font-size: 12px;
  }

  .companies-logos {
    flex-direction: column;
    align-items: center;
  }

  .company-logo {
    max-height: 40px;
  }

  /* Stack left and right lists vertically on small screens */
  .learning-lists,
  .includes-lists {
    flex-direction: column;
  }
}
</style>
