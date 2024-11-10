<template>
  <div class="relative flex flex-col lg:flex-row h-auto lg:h-screen">
    <!-- Right Section (Introduction and About Me Button) -->
    <div class="w-full lg:w-1/2 h-auto bg-black flex flex-col justify-center items-center p-4 text-center text-white">
      <!-- Introduction Section -->
      <h1 class="text-3xl md:text-5xl font-bold mb-4">Hi! I'm John Jerome Bernal</h1>
      <p class="text-lg md:text-2xl mb-10">Software Engineer</p>

      <!-- About Me Button -->
      <button class="mt-8 px-6 py-3 bg-gray-700 text-white rounded-md hover:bg-gray-600">
        <a href="#about">About Me</a>
      </button>
    </div>

    <!-- Left Section (Logo and Image) -->
    <div class="w-full lg:w-1/2 h-auto bg-black flex flex-col justify-center items-center p-4">
      <!-- Logo positioned at the top left -->
      <div class="absolute top-4 left-4 z-10">
        <img alt="Logo" src="./assets/logo.png" class="h-8 w-auto" />
      </div>

      <!-- Centered Image -->
      <div class="mt-8 lg:mt-0 flex justify-center">
        <img alt="John Jerome Bernal" src="./assets/img/jerrr.png" class="object-cover max-w-full h-auto" />
      </div>
    </div>
  </div>

  <!-- About Me Section -->
  <section id="about" class="bg-white py-16 px-4 md:px-16">
    <div class="max-w-7xl mx-auto text-center">
      <h2 class="text-4xl font-semibold text-gray-800 mb-6">About Me</h2>
      <p class="text-lg text-gray-600 mb-4">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac nisi ut turpis malesuada vestibulum eu vel leo. Proin varius, eros ac consectetur condimentum, dui nulla egestas metus, sed aliquet elit magna nec dui. Etiam eleifend velit ut libero eleifend, nec lobortis justo convallis.
      </p>
      <p class="text-lg text-gray-600">
        Sed porttitor lectus ut dolor euismod, ac viverra nunc sollicitudin. Ut ultricies bibendum ipsum, sit amet tincidunt enim auctor et. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Aenean vel augue at nunc sodales tempus.
      </p>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-center py-4 bg-gray-800 text-white">
    Footer
  </footer>
</template>

<style scoped>
/* Additional styling can go here */
</style>
