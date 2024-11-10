<template>
  <div class="instructor-container">
    <!-- Instructor Header -->
    <div class="header">
      <h3>Instructor</h3>
    </div>

    <!-- Instructor Information Section -->
    <div class="instructor-info">
      <div class="instructor-details">
        <span class="instructor-name">TechLink Selenium | DevOps | GenAI</span>
        <span class="instructor-title">Software Architect</span>
      </div>

      <div class="instructor-profile">
        <div class="profile-image">
          <img
            src="https://images.unsplash.com/photo-1730956473717-b1bb69fc595e?q=80&w=1414&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
            alt="Instructor Image"
          />
        </div>

        <!-- Instructor Stats List with Icons -->
        <ul class="instructor-stats">
          <li><span class="icon">⭐</span>4.5 Instructor Rating</li>
          <li><span class="icon">💬</span>22,955 Reviews</li>
          <li><span class="icon">👥</span>300,548 Students</li>
          <li><span class="icon">📚</span>23 Courses</li>
        </ul>
      </div>
    </div>

    <!-- Instructor Philosophy Section -->
    <div class="instructor-philosophy">
      <p>
        Sometimes, reaching out and taking someone's hand is the beginning of a
        journey. We often need someone to help us take the first few steps
        before we get a master's in that move.
      </p>
      <p>
        This is the vision we have behind all of our courses: 'Step by Step'
      </p>
      <ul>
        <li>Start from scratch</li>
        <li>Break down the topic</li>
        <li>Simplify things</li>
        <li>Go step by step</li>
      </ul>
      <p>
        Teaching is our passion, and we design every course so you can start
        from scratch, knowing nothing about a topic and become an expert after
        the course, ready to work on enterprise projects.
      </p>
      <p>
        Do not worry if you do not have any existing knowledge of the subject.
        We will go very basic, step by step.
      </p>
      <p class="start-text">Let's Get Started...</p>
      <p class="signature">FutureTech9</p>
      <div class="support-note">
        ********************************************************************<br />
        All courses under our banner come with lifetime support, and you can ask
        questions whenever you face issues, want to discuss anything, or need my
        suggestions.
        <br />********************************************************************
      </div>
    </div>
  </div>
</template>

<style scoped>
.instructor-container {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 30px auto;
  padding: 20px;
  background-color: #f9f9f9;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.header h3 {
  font-size: 1.75rem;
  color: #333;
  margin-bottom: 15px;
  text-align: center;
}

.instructor-info {
  display: flex;
  flex-direction: column;
  gap: 15px;
  margin-bottom: 30px;
  text-align: center;
}

.instructor-details {
  font-size: 1rem;
  color: #666;
}

.instructor-name {
  font-weight: bold;
  font-size: 1.1rem;
}

.instructor-title {
  font-size: 0.9rem;
  color: #888;
}

.instructor-profile {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
}

.profile-image img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  object-fit: cover;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
}

/* Instructor Stats List Styling */
.instructor-stats {
  list-style: none;
  padding: 0;
  margin: 0;
  color: #555;
  font-size: 0.95rem;
  text-align: left;
}

.instructor-stats li {
  display: flex;
  align-items: center;
  margin-bottom: 8px;
}

.instructor-stats .icon {
  font-size: 1.2rem;
  margin-right: 8px;
}

.instructor-philosophy {
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 3px 8px rgba(0, 0, 0, 0.1);
  color: #333;
}

.instructor-philosophy p {
  margin-bottom: 12px;
  line-height: 1.5;
}

.instructor-philosophy ul {
  margin: 15px 0;
  padding-left: 20px;
  list-style-type: disc;
  color: #555;
}

.instructor-philosophy ul li {
  margin-bottom: 5px;
}

.start-text {
  font-weight: bold;
  color: #2c3e50;
  font-size: 1.1rem;
  margin-top: 20px;
}

.signature {
  font-size: 1rem;
  color: #2980b9;
  text-align: right;
  font-style: italic;
  margin-top: 10px;
}

.support-note {
  color: #444;
  font-size: 0.9rem;
  text-align: center;
  margin-top: 20px;
  padding-top: 10px;
  border-top: 1px solid #ddd;
}
</style>
