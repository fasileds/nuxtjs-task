<template>
  <div class="reviews-container">
    <!-- Course Rating Section -->
    <div class="course-rating">
      <div class="rating-info">
        <i class="icon-star"></i>
        <span class="rating-value">4.4 course rating</span>
        <span class="rating-count">431 ratings</span>
      </div>
    </div>

    <!-- Reviews Section (2 Column Layout) -->
    <div class="reviews-grid">
      <div class="review-card">
        <div class="review-header">
          <div class="review-avatar">
            <img
              src="https://images.unsplash.com/photo-1730956473717-b1bb69fc595e?q=80&w=1414&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
              alt="Reviewer Avatar"
              class="avatar"
            />
          </div>
          <div class="review-info">
            <span class="reviewer-name">Mayank T.</span>
            <div class="review-meta">
              <span class="review-rating">
                <i class="icon-star"></i> 4 stars
              </span>
              <span class="review-date">a week ago</span>
            </div>
          </div>
        </div>
        <div class="review-text">
          <span>
            The way of presenting the topic with theory and practical examples
            makes the course easy to understand. Great course!
          </span>
        </div>
        <div class="helpful-section">
          <span>Helpful?</span>
          <div class="thumbs">
            <button class="thumb-up">
              <i class="icon-thumbs-up"></i>
            </button>
            <button class="thumb-down">
              <i class="icon-thumbs-down"></i>
            </button>
          </div>
        </div>
      </div>

      <div class="review-card">
        <div class="review-header">
          <div class="review-avatar">
            <img
              src="https://plus.unsplash.com/premium_photo-1664541336692-e931d407ba88?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
              alt="Reviewer Avatar"
              class="avatar"
            />
          </div>
          <div class="review-info">
            <span class="reviewer-name">John D.</span>
            <div class="review-meta">
              <span class="review-rating">
                <i class="icon-star"></i> 5 stars
              </span>
              <span class="review-date">2 weeks ago</span>
            </div>
          </div>
        </div>
        <div class="review-text">
          <span>
            Excellent content and teaching style. I was able to grasp difficult
            concepts with ease. Highly recommend!
          </span>
        </div>
        <div class="helpful-section">
          <span>Helpful?</span>
          <div class="thumbs">
            <button class="thumb-up">
              <i class="icon-thumbs-up"></i>
            </button>
            <button class="thumb-down">
              <i class="icon-thumbs-down"></i>
            </button>
          </div>
        </div>
      </div>

      <div class="review-card">
        <div class="review-header">
          <div class="review-avatar">
            <img
              src="https://plus.unsplash.com/premium_photo-1664536392896-cd1743f9c02c?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
              alt="Reviewer Avatar"
              class="avatar"
            />
          </div>
          <div class="review-info">
            <span class="reviewer-name">Sarah L.</span>
            <div class="review-meta">
              <span class="review-rating">
                <i class="icon-star"></i> 3 stars
              </span>
              <span class="review-date">3 weeks ago</span>
            </div>
          </div>
        </div>
        <div class="review-text">
          <span>
            The course was okay, but I feel some areas could be explained in
            more depth. Overall, good value for money.
          </span>
        </div>
        <div class="helpful-section">
          <span>Helpful?</span>
          <div class="thumbs">
            <button class="thumb-up">
              <i class="icon-thumbs-up"></i>
            </button>
            <button class="thumb-down">
              <i class="icon-thumbs-down"></i>
            </button>
          </div>
        </div>
      </div>

      <div class="review-card">
        <div class="review-header">
          <div class="review-avatar">
            <img
              src="https://plus.unsplash.com/premium_photo-1678197937465-bdbc4ed95815?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
              alt="Reviewer Avatar"
              class="avatar"
            />
          </div>
          <div class="review-info">
            <span class="reviewer-name">David K.</span>
            <div class="review-meta">
              <span class="review-rating">
                <i class="icon-star"></i> 4.5 stars
              </span>
              <span class="review-date">1 month ago</span>
            </div>
          </div>
        </div>
        <div class="review-text">
          <span>
            Good course overall. The instructor explains each step clearly and
            the examples are relevant to real-world applications.
          </span>
        </div>
        <div class="helpful-section">
          <span>Helpful?</span>
          <div class="thumbs">
            <button class="thumb-up">
              <i class="icon-thumbs-up"></i>
            </button>
            <button class="thumb-down">
              <i class="icon-thumbs-down"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="show-all-reviews">
      <span>Show all reviews</span>
    </div>
  </div>
</template>

<script>
export default {
  // Add any logic if necessary
};
</script>

<style scoped>
/* General Layout */
.reviews-container {
  max-width: 1000px;
  margin: 20px auto;
  background-color: #f9f9f9;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

/* Course Rating Section */
.course-rating {
  font-size: 1.2rem;
  color: #333;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
}

.rating-info {
  display: flex;
  align-items: center;
  gap: 15px;
}

.icon-star {
  color: #ffcc00;
  font-size: 1.5rem;
}

.rating-value {
  font-size: 1.5rem;
  font-weight: bold;
  color: #333;
}

.rating-count {
  color: #777;
  font-size: 1rem;
  margin-left: 8px;
}

/* Reviews Grid Layout */
.reviews-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.review-card {
  background-color: #fff;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.review-header {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.review-avatar {
  margin-right: 15px;
}

.avatar {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  object-fit: cover;
}

.review-info {
  display: flex;
  flex-direction: column;
}

.reviewer-name {
  font-weight: bold;
  color: #333;
  font-size: 1.1rem;
}

.review-meta {
  display: flex;
  align-items: center;
  font-size: 0.9rem;
  color: #777;
}

.review-rating {
  margin-right: 10px;
  display: flex;
  align-items: center;
}

.icon-star {
  color: #ffcc00;
  margin-right: 5px;
}

.review-date {
  font-style: italic;
  color: #999;
}

/* Review Text */
.review-text {
  margin: 15px 0;
  color: #555;
  font-size: 1rem;
}

/* Helpful Section */
.helpful-section {
  display: flex;
  align-items: center;
  gap: 10px;
}

.helpful-section span {
  font-size: 0.95rem;
  color: #333;
}

.thumbs {
  display: flex;
  gap: 10px;
}

.thumb-up,
.thumb-down {
  background: none;
  border: none;
  cursor: pointer;
  font-size: 1.3rem;
  color: #3498db;
}

.thumb-up:hover,
.thumb-down:hover {
  color: #2980b9;
}

.icon-thumbs-up::before {
  content: "👍";
}

.icon-thumbs-down::before {
  content: "👎";
}
.show-all-reviews {
  display: inline-block;
  padding: 8px 20px;
  margin-top: 20px;
  border: 2px solid rgb(68, 68, 68); /* 2px border */
  border-radius: 5px;
  background-color: #f5f8fa;
  font-weight: bold;
  font-size: 1rem;
  cursor: pointer;
  transition: all 0.3s ease;
  text-align: center;
}

.show-all-reviews span {
  display: inline-block;
}

/* Aligning it to the left */
.show-all-reviews {
  margin-left: 0;
  margin-right: 0;
}
</style>
