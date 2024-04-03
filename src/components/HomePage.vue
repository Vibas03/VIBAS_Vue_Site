<template>
  <div class="home-page">
    <!-- Header Section -->
    <header class="header">
      <div class="profile-container">
        <div class="profile-image"></div>
        <div class="site-info">
          <h1 class="site-title">Tyrone Piolo A. Vibas</h1>
          <p class="site-description">Personal Blog</p>
        </div>
      </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-content">
        <h2 class="welcome-message" id="welcome-message">Welcome to My Blog</h2>
        <div class="explore-message"> <!-- Wrap the text inside a div -->
          <span class="explore-box">Embark on a journey through captivating artistry, thought-provoking articles, and beyond</span>
        </div>
        <router-link to="/about" class="btn">Learn More</router-link> <!-- Modify this line -->
      </div>
    </section>

   <!-- Featured Posts Section -->
<section class="featured-posts">
  <h2>Featured Posts</h2>
  <div class="post-card-container">
    <!-- Featured Post Cards -->
    <div class="post-card">
      <img src="@/assets/tyGalT.jpg" alt="Post Image">
      <h3>Gallery</h3>
      <p>Discover stunning images and captivating moments from around the world.</p> <!-- Updated caption -->
      <router-link to="/gallery" class="btn">Explore</router-link>
    </div>
    <div class="post-card">
      <img src="@/assets/tyGal1.jpg" alt="Post Image">
      <h3>Events</h3>
      <p>Stay updated with the latest events and happenings.</p> <!-- Updated caption -->
      <router-link to="/events" class="btn">Explore</router-link>
    </div>
    <div class="post-card">
      <img src="@/assets/tyGal2.jpg" alt="Post Image">
      <h3>Hobbies</h3>
      <p>Explore my hobbies and interests in detail.</p> <!-- Updated caption -->
      <router-link to="/hobbies" class="btn">Explore</router-link>
    </div>
  </div>
</section>

    <!-- About Section -->
    <section class="about">
      <h2>About Me</h2>
      <p>Hi, I'm Tyrone Piolo A. Vibas, the creator of this blog. I'm passionate about sharing my knowledge and experiences with you through insightful articles and inspiring stories.</p>
      <router-link to="/about" class="btn">Learn More</router-link>
    </section>

    <!-- Newsletter Signup Section -->
    <section class="newsletter">
      <h2>Subscribe to My Newsletter</h2>
      <p>Stay updated with the latest articles and exclusive offers.</p>
      <form>
        <input type="email" placeholder="Enter your email">
        <button type="submit" class="btn">Subscribe</button>
      </form>
    </section>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  mounted() {
    this.animateWelcomeMessage();
  },
  methods: {
    animateWelcomeMessage() {
      const welcomeMessage = document.getElementById('welcome-message');
      const text = welcomeMessage.innerText;
      welcomeMessage.innerHTML = ''; // Clear the original text
      for (let i = 0; i < text.length; i++) {
        const span = document.createElement('span');
        span.textContent = text[i];
        span.style.textShadow = `
        -2px -2px 2px skyblue,   /* Sky Blue */
            2px -2px 2px white,      /* White */
            -2px 2px 2px violet,     /* Violet */
            2px 2px 2px #111         /* Black */
          `; // Sky Blue, White, Violet, Black
        welcomeMessage.appendChild(span);
      }
    }
  }
}
</script>
<style scoped>
/* Your styles */
/* Header Section Styles */
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
}

.profile-container {
  display: flex;
  align-items: center;
}

.profile-image {
  width: 99px;
  height: 150px;
  background-image: url('@/assets/typrof.jpg');
  background-size: cover; /* Ensure the image covers the entire circle */
  border-radius: 50%;
}

.site-info {
  text-align: left;
  margin-left: 20px; /* Adjust the margin as needed */
  cursor: default;
}

.site-title {
  font-size: 2rem;
  margin: 0;
  cursor: default;
}

.site-description {
  margin: 5px 0;
  cursor: default;
}

/* Your existing styles */

/* Welcome Message Styles */
.welcome-message {
  font-size: 3.5rem; /* Adjust the font size as needed */
  display: inline-block;
  transition: font-size 0.3s ease; /* Add transition for font size change */
  cursor: default; /* Set default cursor */
}

/* Hover effect */
.welcome-message:hover {
  font-size: 4rem; /* Increase font size on hover */
  color: #141313; /* Change the text color on hover */
  cursor: pointer; /* Change cursor to pointer on hover */
}

/* Explore Message Styles */
.explore-message {
  font-size: 1.1rem; /* Adjust the font size as needed */
  margin-top: -20px; /* Adjust the margin-top to move the message upward */
  cursor: default;
}

/* Box Styles */
.explore-box {
  background-color: black; /* Background color for the box */
  padding: 5px 10px; /* Adjust padding as needed */
  border-radius: 50px; /* Add border-radius for rounded corners */
}

/* Button Styles */
.btn {
  display: inline-block;
  padding: 10px 20px;
  background-color: #000000;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
  transition: background-color 0.3s ease;
  margin-top: 10px; /* Add margin-top to create space between the button and the text */
}

.btn:hover {
  background-color: #00e6f7; /* Change background color on hover */
}

/* Featured Posts Section Styles */
.featured-posts {
  margin-top: 50px;
  cursor: default;
}

.post-card-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  
}

.post-card {
  padding: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
 
}

.post-card img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 20px;
  cursor: default;
}

.post-card h3 {
  font-size: 1.5rem;
  margin-bottom: 10px;
  cursor: default;
}

.post-card p {
  margin-bottom: 20px;
  cursor: default;
}
/* About Section */
.about {
  cursor: default; /* Set default cursor for the About section */
}

/* Newsletter Signup Section */
.newsletter {
  cursor: default; /* Set default cursor for the Newsletter Signup section */
}
/* Responsive Layout */
/* Featured Post Card Styles */
.post-card {
  padding: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  background-image: url('@/assets/tyGal3.jpg');
  transition: transform 0.3s ease; /* Add transition for smooth scaling */
  cursor: pointer; /* Set cursor to pointer */
}

.post-card:hover {
  transform: scale(1.1); /* Scale up the card on hover */
}

@media (max-width: 768px) {
  .post-card-container {
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  }
}
</style>
