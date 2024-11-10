<template>
  <div class="course-container">
    <h1>
      Google Cloud Platform (GCP) Professional Cloud Architect Certification
    </h1>

    <!-- Description Section -->
    <section class="description">
      <h2>Description</h2>
      <p>
        Google Cloud Platform is one of the fastest-growing cloud service
        platforms offered today that lets you run your applications and data
        workflows at a 'Google-sized' scale.
      </p>
      <p>
        The Google Cloud Certified Professional Cloud Architect certification is
        one of the most highly desired IT certifications out today. It is also
        one of the most challenging exams offered by any cloud vendor today.
        Passing this exam will take many hours of study, hands-on experience,
        and an understanding of a very wide range of GCP topics.
      </p>
      <p>
        Luckily, we're here to help you out! This course is designed to be your
        best single resource to prepare for and pass the exam to become a
        certified Google Cloud Architect.
      </p>
    </section>

    <!-- Show More / Show Less Toggle -->
    <div v-if="isExpanded" class="additional-content">
      <!-- Why do a Google Cloud Certification Section -->
      <section class="why-google-certification">
        <h2>Why should you do a Google Cloud Certification?</h2>
        <ul>
          <li>
            89% of Google Cloud certified individuals are more confident about
            their cloud skills.
          </li>
          <li>
            GCP Cloud Architect was the highest paying certification of 2020 and
            2019.
          </li>
          <li>
            More than 1 in 4 of Google Cloud certified individuals took on more
            responsibility or leadership roles at work.
          </li>
        </ul>
      </section>

      <!-- Why Google Cloud Architect Certification Section -->
      <section class="why-cloud-architect-certification">
        <h2>
          Why should you aim for Google Cloud - GCP Cloud Architect
          Certification?
        </h2>
        <ul>
          <li>
            Google Cloud Professional Cloud Architect certification helps you
            gain an understanding of cloud architecture and Google Cloud
            Platform.
          </li>
          <li>
            As a Cloud Architect, you will learn to design, develop, and manage
            robust, secure, scalable, highly available, and dynamic solutions to
            drive business objectives.
          </li>
        </ul>
      </section>

      <!-- Exam Details Section -->
      <section class="exam-details">
        <h2>The Google Cloud Certified - Professional Cloud Architect Exam</h2>
        <p>The exam assesses your ability to:</p>
        <ul>
          <li>Design and architect a GCP solution architecture.</li>
          <li>Manage and provision the GCP solution infrastructure.</li>
          <li>Design for security and compliance.</li>
          <li>Analyze and optimize technical and business processes.</li>
          <li>Manage implementations of Google Cloud architecture.</li>
          <li>Ensure solution and operations reliability.</li>
        </ul>
      </section>

      <!-- For Whom Section -->
      <section class="for-whom">
        <h2>Who this course is for:</h2>
        <ul>
          <li>
            You want to start your Cloud Journey with Google Cloud Platform.
          </li>
          <li>
            You want to become a Google Cloud Certified Professional Cloud
            Architect.
          </li>
        </ul>
      </section>
    </div>

    <!-- Toggle Text Link -->
    <p @click="toggleExpand" class="show-more-link">
      {{ isExpanded ? "Show Less" : "Show More" }}
    </p>
  </div>
</template>

<script>
export default {
  name: "GoogleCloudCertificationCourse",
  data() {
    return {
      // Boolean to toggle expanded content
      isExpanded: false,
    };
  },
  methods: {
    // Toggle the visibility of additional content
    toggleExpand() {
      this.isExpanded = !this.isExpanded;
    },
  },
};
</script>

<style scoped>
.course-container {
  font-family: Arial, sans-serif;
  margin: 20px;
  padding: 20px;
}

h1 {
  font-size: 1.5rem; /* Decreased font size */
  font-weight: bold;
  color: black;
  margin-bottom: 20px;
}

h2 {
  font-size: 1.2rem; /* Decreased font size */
  font-weight: bold;
  color: black;
  margin-top: 20px;
  margin-bottom: 10px;
}

p,
ul {
  font-size: 0.9rem; /* Decreased font size */
  color: black;
  margin-bottom: 10px;
}

ul {
  padding-left: 20px;
}

ul li {
  margin-bottom: 5px;
}

section {
  margin-bottom: 30px;
}

/* Show More / Show Less Text Link */
.show-more-link {
  color: #ac2eb3;
  font-weight: bold;
  cursor: pointer;
  font-size: 0.9rem; /* Decreased font size */
  text-decoration: underline;
}

.show-more-link:hover {
  color: #3498db;
}

/* Additional Content Section */
.additional-content {
  display: block;
}
</style>
