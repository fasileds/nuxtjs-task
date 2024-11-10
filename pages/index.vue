<template>
  <div>
    <Top />

    <!-- Conditionally render Navbar or Sticky -->
    <Navbar v-if="!scrolled" />
    <Sticky v-if="scrolled" />

    <Header />
    <div class="main-content">
      <Course />
      <SideBar />
    </div>
    <Footer />
  </div>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from "vue";

const scrolled = ref(false);

// Function to track page scroll
const handleScroll = () => {
  scrolled.value = window.scrollY > 100; // You can adjust this threshold as needed
};

// Adding the scroll event listener when the component is mounted
onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

// Removing the scroll event listener when the component is unmounted
onBeforeUnmount(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style scoped>
.main-content {
  display: flex;
  gap: 20px;
  padding: 20px;
}
.SideBar {
  flex: 1 1 250px;
  max-width: 300px;
}

.Course {
  flex: 3;
}
</style>
