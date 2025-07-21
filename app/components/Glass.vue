<template>
  <div class="h-screen w-screen flex justify-center items-center">
    <div class="glass">
      <h1>Glassmorphism</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia
        laborum inventore nulla illum, eaque sint culpa. Repellat aliquid nemo
        vero nesciunt placeat voluptate aspernatur sapiente? Dolorum
        necessitatibus officiis nobis laboriosam!
      </p>
    </div>
  </div>
</template>

<style lang="css" scoped>
.glass {
  width: 80%;
  height: 80vh;
  padding: 2rem;
  background-color: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.4);
  border-right-color: rgba(255, 255, 255, 0.2);
  border-bottom-color: rgba(255, 255, 255, 0.2);
  border-radius: 10px;
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  line-height: normal;
}

.glass h1 {
  text-align: center;
  color: #fff;
  font-size: 50px;
  font-weight: bold;
  letter-spacing: 0.06em;
}

.glass p {
  margin-top: 20px;
  color: #fff;
  font-size: 16px;
}
</style>
