<template>
  <div class="flex-container">
    <CourseContent />
    <Learn />
    <CourseContetents />
    <Description />
    <StudentsAlsoBought />
    <FrequentlyBoughtCourses />
    <Instructor />
    <CourseRiview />
    <MoreCourses />
  </div>
</template>

<script>
import StudentsAlsoBought from "./StudentsAlsoBought.vue";
import CourseContent from "./CourseContent.vue";
import CourseContetents from "./CourseContetents.vue";
import Description from "./Description.vue";
import Learn from "./Learn.vue";
import FrequentlyBoughtCourses from "./FrequentlyBoughtCourses.vue";
import Instructor from "./Instructor.vue";
import CourseRiview from "./CourseRiview.vue";
import MoreCourses from "./MoreCourses.vue";
</script>

<style scoped>
.flex-container {
  display: flex;
  flex-direction: column;
  gap: 20px; /* Adds space between the two components */
  align-items: center; /* Centers the components horizontally */
  padding: 20px;
}
</style>
