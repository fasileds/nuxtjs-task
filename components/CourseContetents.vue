<template>
  <div class="course-content">
    <!-- Course Header Section -->
    <div class="course-header">
      <h3 class="course-title">Course Content</h3>
    </div>

    <!-- Course Stats Section -->
    <div class="course-stats">
      <div class="stats">
        <span class="section-details">
          25 Sections • 139 Lectures • 22h 20m Total Length
        </span>
      </div>
      <div class="expand-section">
        <span class="expand-all">Expand All Sections</span>
      </div>
    </div>

    <!-- Sections Placeholder with Expandable List -->
    <div class="sections-placeholder">
      <!-- Section 1 -->
      <div class="section-item" @click="toggleSection(0)">
        <span class="icon" :class="{ expanded: isExpanded(0) }">
          <i
            :class="isExpanded(0) ? 'fas fa-chevron-down' : 'fas fa-chevron-up'"
          ></i>
        </span>
        GCP Professional Cloud Architect: Course Introduction
        <span class="lecture-info">5 Lectures • 19min</span>
      </div>
      <div v-if="isExpanded(0)" class="section-dropdown">
        <ul>
          <li>Lecture 1: Introduction to GCP <span>05:26</span></li>
          <li>Lecture 2: Setting up GCP Account <span>05:26</span></li>
          <li>Lecture 3: Exploring GCP Services <span>05:26</span></li>
          <li>Lecture 4: GCP Networking <span>05:26</span></li>
          <li>Lecture 5: Exam Preparation <span>05:26</span></li>
        </ul>
      </div>

      <!-- Section 2 -->
      <div class="section-item" @click="toggleSection(1)">
        <span class="icon" :class="{ expanded: isExpanded(1) }">
          <i
            :class="isExpanded(1) ? 'fas fa-chevron-down' : 'fas fa-chevron-up'"
          ></i>
        </span>
        GCP Infrastructure: Virtual Machines and Networking
        <span class="lecture-info">7 Lectures • 45min</span>
      </div>
      <div v-if="isExpanded(1)" class="section-dropdown">
        <ul>
          <li>Lecture 1: Virtual Machines in GCP <span>06:15</span></li>
          <li>Lecture 2: Networking in GCP <span>05:20</span></li>
          <li>Lecture 3: Configuring Firewalls <span>07:30</span></li>
          <li>Lecture 4: VPCs and Subnets <span>05:50</span></li>
          <li>Lecture 5: Load Balancing in GCP <span>05:40</span></li>
          <li>Lecture 6: GCP Security Best Practices <span>06:00</span></li>
          <li>
            Lecture 7: Preparing for the Networking Exam <span>07:10</span>
          </li>
        </ul>
      </div>

      <!-- Section 3 -->
      <div class="section-item" @click="toggleSection(2)">
        <span class="icon" :class="{ expanded: isExpanded(2) }">
          <i
            :class="isExpanded(2) ? 'fas fa-chevron-down' : 'fas fa-chevron-up'"
          ></i>
        </span>
        GCP Storage Solutions and Management
        <span class="lecture-info">4 Lectures • 30min</span>
      </div>
      <div v-if="isExpanded(2)" class="section-dropdown">
        <ul>
          <li>Lecture 1: Introduction to GCP Storage <span>08:10</span></li>
          <li>Lecture 2: Cloud Storage Buckets <span>06:20</span></li>
          <li>Lecture 3: Databases in GCP <span>07:50</span></li>
          <li>
            Lecture 4: GCP Storage Security and Best Practices
            <span>08:10</span>
          </li>
        </ul>
      </div>

      <!-- Section 4 -->
      <div class="section-item" @click="toggleSection(3)">
        <span class="icon" :class="{ expanded: isExpanded(3) }">
          <i
            :class="isExpanded(3) ? 'fas fa-chevron-down' : 'fas fa-chevron-up'"
          ></i>
        </span>
        GCP Security: Best Practices and Tools
        <span class="lecture-info">6 Lectures • 40min</span>
      </div>
      <div v-if="isExpanded(3)" class="section-dropdown">
        <ul>
          <li>
            Lecture 1: GCP Security Overview
            <span class="lecture-time">07:30</span>
          </li>
          <li>Lecture 2: IAM in GCP <span class="lecture-time">06:50</span></li>
          <li>
            Lecture 3: Cloud Security Tools
            <span class="lecture-time">07:10</span>
          </li>
          <li>
            Lecture 4: Secure Access and Identity
            <span class="lecture-time">06:00</span>
          </li>
          <li>
            Lecture 5: Monitoring and Auditing in GCP
            <span class="lecture-time">06:30</span>
          </li>
          <li>
            Lecture 6: Preparing for the Security Exam
            <span class="lecture-time">06:10</span>
          </li>
        </ul>
      </div>
    </div>
    <div class="more-sections">15 more sections</div>
  </div>
</template>

<script setup>
// Importing required composition API function
import { ref } from "vue";

// Toggle state for each section
const expandedSections = ref([false, false, false, false]);

// Toggle function to handle expand/collapse
function toggleSection(index) {
  expandedSections.value[index] = !expandedSections.value[index];
}

// Check if a section is expanded
function isExpanded(index) {
  return expandedSections.value[index];
}
</script>

<style scoped>
.course-content {
  width: 700px;
  margin: 0;
  padding: 30px;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  text-align: left;
}

.course-header {
  margin-bottom: 20px;
}

.course-title {
  font-size: 36px;
  font-weight: bold;
  color: #333;
  letter-spacing: 1px;
}

.course-stats {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  margin-bottom: 30px;
}

.stats {
  font-size: 16px;
  color: #555;
}

.section-details {
  font-size: 16px;
  color: #555;
  font-weight: normal;
}

.expand-section {
  cursor: pointer;
  margin-left: 20px;
}

.expand-all {
  font-size: 14px;
  color: #5022c3;
  font-weight: bold;
  transition: color 0.3s;
}

.expand-all:hover {
  color: #370b80;
  text-decoration: underline;
}

/* Sections Placeholder */
.sections-placeholder {
  background-color: #fff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  min-height: 150px;
  color: #aaa;
}

.section-item {
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: 16px;
  color: #333;
  padding: 10px 0;
  border-bottom: 1px solid #ddd;
}

.icon {
  margin-right: 10px;
  transition: transform 0.3s;
}

.icon i {
  font-size: 18px;
  color: #5022c3;
}

.icon.expanded i {
  transform: rotate(180deg);
}

.lecture-info {
  margin-left: auto;
  font-size: 14px;
  color: #777;
}

.section-dropdown {
  margin-top: 10px;
  padding-left: 20px;
  font-size: 14px;
}

.section-dropdown ul {
  list-style-type: none;
  padding-left: 0;
}

.section-dropdown li {
  display: flex;
  justify-content: space-between;
  padding: 5px 0;
  font-size: 14px;
}

.lecture-time {
  margin-left: 10px; /* Space between the text and time */
  color: #777;
}
.more-sections {
  display: inline-block;
  padding: 10px 20px;
  width: 90%;
  border: 1px solid rgb(88, 88, 88);
  background-color: #f4f0ff;
  font-size: 16px;
  font-weight: bold;
  text-align: center;
  cursor: pointer;
  transition: all 0.3s ease;
  margin-top: 30px;
}

/* Hover effect */
.more-sections:hover {
  border-color: #370b80; /* Darker border on hover */
  transform: translateY(-2px); /* Slightly lift the element */
}

/* Focus effect */
.more-sections:focus {
  outline: none; /* Removes default outline */
  box-shadow: 0 0 0 3px rgba(80, 34, 195, 0.3); /* Custom focus outline */
}

/* Mobile Responsiveness */
@media (max-width: 768px) {
  .course-content {
    padding: 15px;
  }

  .course-title {
    font-size: 28px;
  }

  .section-details {
    font-size: 14px;
  }

  .expand-all {
    font-size: 12px;
  }
}
</style>
