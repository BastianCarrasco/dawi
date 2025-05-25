<template>
  <div class="about">
    <h1>About</h1>
    <p>This is the About page.</p>
    
    <div class="button-container">
      <button class="box z-axis" @click="$router.push('/')">
        Eje Z (normal)
      </button>
      
      <button class="box x-axis" @click="$router.push('/')">
        Eje X (frontal)
      </button>
      
      <button class="box y-axis" @click="$router.push('/')">
        Eje Y (lateral)
      </button>
    </div>
  </div>
</template>

<script setup>
// No se necesita lógica adicional
</script>

<style scoped>
.about {
  padding: 2rem;
  text-align: center;
}

.button-container {
  display: flex;
  gap: 20px;
  justify-content: center;
  margin-top: 30px;
}

.box {
  padding: 20px 20px;
  background-color: #42b983;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: transform 0.8s ease;
}

.z-axis:hover {
  transform: rotateZ(360deg);
  background-color: #3aa876;
}

.x-axis:hover {
  transform: rotateX(360deg);
  background-color: #ff7b00;
}

.y-axis:hover {
  transform: rotateY(360deg);
  background-color: #007bff;
}
</style>