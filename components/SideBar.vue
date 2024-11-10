<template>
  <div class="container">
    <div class="sidebar">
      <img
        src="https://images.unsplash.com/photo-1557804483-ef3ae78eca57?q=80&w=1488&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
        alt=""
      />

      <div class="tabs">
        <div
          class="tab"
          :class="{ active: activeTab === 'personal' }"
          @click="setActiveTab('personal')"
        >
          Personal
        </div>
        <div
          class="tab"
          :class="{ active: activeTab === 'teams' }"
          @click="setActiveTab('teams')"
        >
          Teams
        </div>
      </div>
      <div
        v-show="activeTab === 'personal'"
        class="content personal sticky-content"
      >
        <h2>Subscribe to Udemy’s top courses</h2>
        <p>
          Get this course, plus 12,000+ of our top-rated courses, with Personal
          Plan. <span> Learn more</span>
        </p>
        <div class="personal-plan">
          <button>Try Personal Plan For Free</button>
          <span class="pricing">
            Starting at $10.00 per month after trial. Cancel anytime
          </span>
        </div>
        <span class="or-divider">
          <hr class="left-line" />
          <span>or</span>
          <hr class="right-line" />
        </span>
        <h3>$49.99</h3>
        <div class="add-to-cart">Add To Cart</div>
        <span class="guarantee">
          30-Day Money-Back Guarantee |
          <span> Full Lifetime Access</span>
        </span>
        <div class="additional-options">
          <span>Share</span>
          <span>Gift this course</span>
          <span>Apply coupon</span>
        </div>
      </div>
      <div v-show="activeTab === 'teams'" class="content teams sticky-content">
        <h1>Udemy <span>Business</span></h1>
        <p>
          Subscribe to this course and 27,000+ top‑rated Udemy courses for your
          organization.
        </p>
        <button>Try Udemy Business</button>
        <ul>
          <li><i class="fas fa-users"></i> For teams of 2 or more users</li>
          <li><i class="fas fa-cogs"></i> 27,000+ fresh & in-demand courses</li>
          <li>
            <i class="fas fa-chalkboard-teacher"></i> Learning Engagement tools
          </li>
          <li><i class="fas fa-key"></i> SSO and LMS Integrations</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      activeTab: "personal",
    };
  },
  methods: {
    setActiveTab(tab) {
      this.activeTab = tab;
    },
  },
};
</script>

<style scoped>
.container {
  display: flex;
  justify-content: flex-end;
  margin-top: -350px;
}
.sidebar {
  width: 300px;
  padding: 20px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  display: flex;
  flex-direction: column;
  gap: 30px;
  margin-right: 100px;
  background-color: white;
}

.video-preview {
  width: 100%;
  border-radius: 12px;
  margin-bottom: 20px;
}
.tabs {
  display: flex;
  gap: 15px;
  justify-content: center;
  border-bottom: 2px solid #ccc;
  padding-bottom: 15px;
}
.tab {
  color: #6f42c1;
  font-size: 18px;
  font-weight: 600;
  cursor: pointer;
  text-align: center;
  padding: 10px;
  transition: color 0.3s ease, transform 0.3s ease;
}

.tab:hover {
  color: #5022c3;
  transform: translateY(-3px);
}

.tab.active {
  color: #5022c3;
  border-bottom: 4px solid #5022c3;
}
.content.personal {
  background-color: #fff;
  padding: 20px;
  font-size: 16px;
  color: #333;
  border-radius: 10px;
}
.sticky-content {
  position: sticky;
  top: 0;
  z-index: 10;
  padding-top: 20px;
}

.content.personal h2 {
  font-size: 26px;
  color: #5022c3;
  margin-bottom: 20px;
}

.content.personal p {
  margin-bottom: 20px;
  font-size: 16px;
  color: #555;
}

.content.personal button {
  background-color: #5022c3;
  color: white;
  padding: 12px 22px;
  border: none;
  cursor: pointer;
  font-size: 16px;
  transition: background-color 0.3s ease;
  border-radius: 5px;
}

.content.personal button:hover {
  background-color: #6f42c1;
}

.personal-plan {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  margin-bottom: 20px;
}

.pricing {
  font-size: 14px;
  color: #555;
  text-align: center;
}

.or-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  margin: 20px 0;
}

.left-line,
.right-line {
  width: 40%;
  border-top: 2px solid #ccc;
}

.or-divider span {
  font-size: 16px;
  color: #333;
}

.guarantee {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  font-size: 12px;
  color: #555;
}

.add-to-cart {
  padding: 10px;
  border: 2px solid;
  text-align: center;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.add-to-cart:hover {
  background-color: #6f42c1;
}

.additional-options span {
  margin-right: 15px;
  color: #5022c3;
  font-size: 14px;
  cursor: pointer;
  border-bottom: 2px solid transparent;
  transition: all 0.3s ease;
}

.additional-options span:hover {
  color: #6f42c1;
  border-bottom: 2px solid #5022c3;
}

.content.teams {
  background-color: #fff;
  padding: 20px;
  font-size: 16px;
  color: #333;
  border-radius: 10px;
}

.content.teams h1 {
  font-size: 28px;
  color: #5022c3;
  margin-bottom: 20px;
}

.content.teams p {
  margin-bottom: 20px;
  font-size: 16px;
  color: #555;
}

.content.teams button {
  background-color: #5022c3;
  color: white;
  padding: 12px 22px;
  border: none;
  cursor: pointer;
  font-size: 16px;
  transition: background-color 0.3s ease;
  border-radius: 5px;
}

.content.teams button:hover {
  background-color: #6f42c1;
}
.content.teams ul {
  list-style-type: none;
  padding-left: 0;
  font-size: 14px;
  color: #555;
}

.content.teams ul li {
  margin-bottom: 12px;
  display: flex;
  align-items: center;
  gap: 10px;
}

.content.teams ul li i {
  color: #5022c3;
  font-size: 20px;
}
</style>
