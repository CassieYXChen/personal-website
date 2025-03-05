<template>
  <div class="home-container">
    <div class="content">
      <h1 class="greeting">
        <span class="hi">Hi!</span>
        <span class="name">I'm Cassie Chen</span>
      </h1>
      <p class="details">
        <!-- Replace this with your actual details -->
        Computer Science @ The Chinese University of Hong Kong
      </p>
    </div>
  </div>
</template>

<style scoped>
.home-container {
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #ffffff;
  padding: 2rem;
}

.content {
  text-align: center;
  animation: fadeIn 1s ease-out;
}

.greeting {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  margin-bottom: 2rem;
}

.hi {
  font-size: 3rem;
  font-weight: 700;
  color: #42b883; /* Vue.js green, you can change this */
}

.name {
  font-size: 4.5rem;
  font-weight: 800;
  color: #2c3e50;
}

.details {
  font-size: 1.5rem;
  color: #666;
  font-weight: 500;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 768px) {
  .hi {
    font-size: 2rem;
  }
  
  .name {
    font-size: 3rem;
  }
  
  .details {
    font-size: 1.25rem;
  }
}
</style>