<template>
  <div class="events-container">
    <h2>Events</h2>
    <div class="event-card">
      <div class="event-image">
        <img src="@/assets/tyGall.jpg" alt="FDA Philippines poster compitition">
      </div>
      <div class="event-info">
        <h3>Realistic Fantasy Illustration Dwarf</h3>
        <p>a dwarf with intricate details capturing both the fantastical elements of dwarven folklore and the nuanced realism of human anatomy and expression.</p>
      </div>
    </div>
    <div class="event-card">
      <div class="event-image">
        <img src="@/assets/tyGaller.jpg" alt="Davao Region Poster Competition">
      </div>
      <div class="event-info">
        <h3>Samurai</h3>
        <p>Embodying discipline and honor, is a skilled warrior of feudal Japan, guided by the code of bushido.</p>
      </div>
    </div>
    <div class="event-card">
      <div class="event-image">
        <img src="@/assets/tyGalT.jpg" alt="Esports Tournament">
      </div>
      <div class="event-info">
        <h3>Esports Tournament (PSITS)</h3>
        <p>A competitive gaming event featuring various esports titles.</p>
      </div>
    </div>
  </div>
</template>

<style>
.events-container {
  text-align: center;
  margin-top: 50px;
}

.events-container h2 {
  margin-bottom: 30px;
}

.event-card {
  display: flex;
  flex-direction: row; 
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  max-width: 600px; 
  margin: 0 auto; 
}

.event-card:hover {
  transform: translateY(-5px);
}

.event-image {
  width: 40%; 
  overflow: hidden;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
}

.event-image img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.event-info {
  width: 60%; 
  padding: 20px;
  background-color: #000000; 
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}

.event-info h3 {
  margin-top: 0;
}

.event-info p {
  margin-bottom: 0;
}


</style>