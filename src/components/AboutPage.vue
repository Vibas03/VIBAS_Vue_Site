<template>
  <div class="about-page">
    <div class="about-content">
      <h1>About Me</h1>
      <div class="profile-details">
        <div class="profile-image"></div>
        <div class="profile-info">
          <h2>Tyrone Piolo A. Vibas</h2>
          <p>E-sports Proplayer, Hacker</p>
          <p>Studied at Jose Maria College</p>
          <p>3rd year college BSIT student</p>
          <p>Age: 22 </p>
          <p>Address: Purok 8 Communal, Buhangin, Davao City</p>
          <p>Follow me on social media:</p>
          <div class="social-icons"> <a href="#"><img src="@/assets/fb.webp" alt="Facebook Icon"></a> <a href="#"><img src="@/assets/insta.png" alt="Instagram Icon"></a> <a href="#"><img src="@/assets/twitter.png" alt="Twitter Icon"></a> <a href="#"><img src="@/assets/linkin.webp" alt="LinkedIn Icon"></a> <a href="#"><img src="@/assets/tiktok.webp" alt="TikTok Icon"></a> </div> </div> </div> </div> </div> </template>

<script>
export default {
  name: 'AboutPage',
}
</script>

<style scoped>
.about-page {
  padding: 50px;
  text-align: center;
  cursor: default;
}

.about-content {
  max-width: 800px;
  margin: 0 auto;
  cursor: default;
}

.profile-details {
  background-color: rgba(0, 0, 0, 0.9); 
  border-radius: 20px;
  padding: 30px;
  margin: 0 auto 30px; 
  max-width: 600px; 
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  text-align: center; 
}

.profile-details h2 {
  margin-bottom: 20px;
}

.profile-details p {
  line-height: 1.5;
}

.profile-image {
  width: 150px;
  height: 200px;
  background-image: url('@/assets/typrof.jpg');
  background-size: cover;
  border-radius: 20px;
  margin: 0 auto 20px; 
}

.profile-info {
  text-align: center; 
}

.profile-info h2 {
  font-size: 2.5rem;
  margin-bottom: 10px;
}

.profile-info p {
  font-size: 1.2rem;
  margin-bottom: 15px;
}

.social-icons {
  display: flex;
  justify-content: center; 
  margin-top: 20px;
}

.social-icons a {
  margin-right: 10px;
}

.social-icons img {
  width: 30px;
  height: auto;
}

.social-icons a:last-child {
  margin-right: 0;
}

</style>