<template>
  <div class="top">
    <div class="content">
      <div class="textPart">
        <span class="highlight">New-learner offer |</span>
        Courses from $10.99. Click the button to see savings.
        <span class="timer"
          >Ends in {{ timeLeft.hours }}h {{ timeLeft.minutes }}m
          {{ timeLeft.seconds }}s</span
        >
      </div>
      <div class="button">
        <button @click="redeemOffer">Click to Redeem</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

const timeLeft = ref({ hours: 5, minutes: 0, seconds: 0 });

function startCountdown() {
  const interval = setInterval(() => {
    if (timeLeft.value.seconds > 0) {
      timeLeft.value.seconds--;
    } else if (timeLeft.value.minutes > 0) {
      timeLeft.value.seconds = 59;
      timeLeft.value.minutes--;
    } else if (timeLeft.value.hours > 0) {
      timeLeft.value.minutes = 59;
      timeLeft.value.seconds = 59;
      timeLeft.value.hours--;
    } else {
      clearInterval(interval);
    }
  }, 1000);
}

onMounted(() => {
  startCountdown();
});

function redeemOffer() {
  alert("Offer redeemed!");
}
</script>

<style scoped>
.top {
  background-color: #f0edbc;
  padding: 15px 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
}

.content {
  display: flex;
  align-items: center;
  gap: 20px;
}

.textPart {
  font-size: 18px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  color: #333;
}

.highlight {
  font-weight: bold;
  margin-right: 4px;
}

.timer {
  font-weight: bold;

  display: block;
  margin-top: 6px;
  font-size: 25px;
}

.button button {
  background-color: #8b25c7;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 8px;
  font-size: 16px;
  font-weight: 600;
  height: 45px;
  cursor: pointer;
  transition: transform 0.2s ease, background-color 0.3s ease;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
}

.button button:hover {
  background-color: #6f1d9f;
  transform: scale(1.05);
}

.button button:active {
  transform: scale(0.98);
}
</style>
