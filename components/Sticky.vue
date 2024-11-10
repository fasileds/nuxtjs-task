<template>
  <div class="course-container">
    <span class="course-title">
      Google Cloud Professional Cloud Architect: GCP Certification
    </span>
    <div class="course-details">
      <div class="best-seller">
        <span>Best Seller</span>
      </div>
      <span class="rating"> 4.4 star icon <span>(431 ratings)</span> </span>
      <span class="students-count">17,694 students</span>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.course-container {
  background-color: #2b2f31;
  padding: 20px;
  border-radius: 8px;
  color: white;
  width: 100%;
  max-width: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  box-sizing: border-box;
  font-family: "Arial", sans-serif;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);

  position: sticky;
  top: 20px;
  z-index: 1000;
}
.course-title {
  font-weight: bold;
  font-size: 1.5rem;
  margin-bottom: 10px;
  display: block;
  width: 100%;
}

.course-details {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: flex-start;
  gap: 20px;
  width: 100%;
}

.best-seller {
  background-color: #ff9800;
  color: white;
  padding: 5px 12px;
  font-size: 1rem;
  font-weight: bold;
  border-radius: 5px;
}
.rating,
.students-count {
  font-size: 1rem;
}

.rating span {
  color: #ff9800;
}
</style>
