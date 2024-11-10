<template>
  <div class="container">
    <div class="header">
      <span>
        Prepare for your certifications with these courses.
        <span class="learn-more"> Learn more </span>
      </span>
    </div>

    <!-- Content Section -->
    <div class="content">
      <!-- Loop over courses and display only the first two initially -->
      <div
        v-for="(course, index) in visibleCourses"
        :key="course.id"
        class="course-info"
      >
        <div class="image-container">
          <img class="course-image" :src="course.image" alt="Course Image" />
        </div>
        <div class="text-content">
          <div class="course-title">{{ course.title }}</div>
          <div class="course-provider">{{ course.provider }}</div>
        </div>
      </div>
    </div>

    <!-- Show More Button -->
    <div class="show-more" @click="toggleShowMore">
      {{ showMore ? "Show less" : "Show more" }}
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showMore: false, // To control whether to show more courses
      courses: [
        {
          id: 1,
          title: "Professional Cloud Architect",
          provider: "Issued by Google Cloud",
          image:
            "https://images.unsplash.com/photo-1730461749751-657b4af6deb5?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
        },
        {
          id: 2,
          title: "AWS Solutions Architect",
          provider: "Issued by Amazon Web Services",
          image:
            "https://images.unsplash.com/photo-1602085883813-4fd38ac7e4e4?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3",
        },
        {
          id: 3,
          title: "Microsoft Azure Architect",
          provider: "Issued by Microsoft",
          image:
            "https://images.unsplash.com/photo-1511200363701-33b2a5679cf6?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3",
        },
        {
          id: 4,
          title: "Certified Kubernetes Administrator",
          provider: "Issued by Cloud Native Computing Foundation",
          image:
            "https://images.unsplash.com/photo-1581091012769-d9f5dba19c62?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3",
        },
      ],
    };
  },
  computed: {
    // Show only the first 2 courses if 'showMore' is false, otherwise show all
    visibleCourses() {
      return this.showMore ? this.courses : this.courses.slice(0, 2);
    },
  },
  methods: {
    // Toggle between showing more or less courses
    toggleShowMore() {
      this.showMore = !this.showMore;
    },
  },
};
</script>

<style scoped>
.container {
  border: 1px solid #ddd;
  padding: 20px;
  border-radius: 12px;
  max-width: 550px;
  margin: 0 auto;
  background-color: #f9f9f9;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}
.header {
  margin-bottom: 20px;
  font-size: 18px;
  color: #333;
  font-weight: 600;
  text-align: center;
}

.learn-more {
  color: #5022c3;
  cursor: pointer;
  font-weight: bold;
}

.learn-more:hover {
  text-decoration: underline;
}

.content {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.course-info {
  display: flex;
  gap: 15px;
  align-items: center;
  padding: 15px;
  border-radius: 8px;
  background-color: #fff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.course-info:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

.image-container {
  width: 80px;
  height: 80px;
  overflow: hidden;
  border-radius: 50%;
  border: 2px solid #5022c3;
}

.course-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.text-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.course-title {
  font-size: 18px;
  font-weight: 600;
  color: #5022c3;
  margin-bottom: 5px;
}

.course-provider {
  font-size: 14px;
  color: #777;
}

/* Show more button */
.show-more {
  margin-top: 20px;
  text-align: center;
  font-size: 16px;
  color: #5022c3;
  cursor: pointer;
  font-weight: bold;
}

.show-more:hover {
  text-decoration: underline;
}
</style>
