<template>
  <div class="hobbies-list">
    <div class="title-container">
      <h1>My HobbiesList</h1>
    </div>
    <div class="hobbies-container">
      <div class="hobby-item">
        <div class="image-wrapper">
          <img src="@/assets/tyTravel.jpg" alt="Hobby 1">
        </div>
        <div class="overlay">
          <h2>Art</h2>
        </div>
      </div>
      <!-- Repeat this structure for other hobby items -->
      <!-- Example for hobby 2 -->
      <div class="hobby-item">
        <div class="image-wrapper">
          <img src="@/assets/tySports.jpg" alt="Hobby 2">
        </div>
        <div class="overlay">
          <h2>Playing Mobile Legends</h2>
        </div>
      </div>
      <!-- Repeat until hobby 8 -->
      <div class="hobby-item">
        <div class="image-wrapper">
          <img src="@/assets/tyChamp.jpg" alt="Hobby 3">
        </div>
        <div class="overlay">
          <h2>PC Games</h2>
        </div>
      </div>
      <div class="hobby-item">
        <div class="image-wrapper">
          <img src="@/assets/MLtourna.jpg" alt="Hobby 4">
        </div>
        <div class="overlay">
          <h2>Nature</h2>
        </div>
      </div>
     
      <div class="hobby-item">
        <div class="image-wrapper">
          <img src="@/assets/tydog.jpg" alt="Hobby 6">
        </div>
        <div class="overlay">
          <h2>Watching Kdrama</h2>
        </div>
      </div>
      <div class="hobby-item">
        <div class="image-wrapper">
          <img src="@/assets/typoster.jpg" alt="Hobby 7">
        </div>
        <div class="overlay">
          <h2>Watching Anime</h2>
        </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'HobbiesList',
}
</script>

<style>
/* Add styles for homepage */
.hobbies-list {
  text-align: center;
  background-image: url('@/assets/tyBG.jpg');
  background-size: cover;
  background-position: center;
  color: #fff;
  padding: 20px;
  cursor: default;
}

.title-container {
  display: inline-block;
  background-color: rgba(0, 0, 0, 0.8);
  padding: 10px;
  border-radius: 10px;
  margin-bottom: 20px;
}

.title-container h1 {
  margin: 0;
}

.hobbies-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
}

.hobby-item {
  position: relative;
  overflow: hidden;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease;
}

.hobby-item:hover {
  transform: scale(1.05);
}

.image-wrapper {
  overflow: hidden;
  border-radius: 10px;
  width: 100%;
  height: 100%;
}

.image-wrapper img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.hobby-item:hover .overlay {
  opacity: 1;
}

.overlay h2 {
  color: #fff;
  font-weight: bold;
  font-size: 20px;
}
</style>
