<template>
  <div class="relative flex flex-col lg:flex-row h-auto lg:h-screen">
    <!-- Right Section (Introduction and About Me Button) -->
    <div class="w-full lg:w-1/2 h-auto bg-black flex flex-col justify-center items-center p-4 text-center text-white">
      <!-- Introduction Section -->
      <h1 class="text-3xl md:text-5xl font-bold mb-4 font-mono">Hi! I'm Jerome Bernal</h1>
      <p class="text-lg md:text-2xl mb-10 font-bold font-mono">Software Engineer</p>

      <!-- About Me Button -->
      <button class="mt-8 px-6 py-3 bg-gray-700 text-white rounded-md hover:bg-gray-600" onclick="document.getElementById('about').scrollIntoView({ behavior: 'smooth' })">
        About Me
      </button>
    </div>

    <!-- Left Section (Image) -->
    <div class="w-full lg:w-1/2 h-auto bg-black flex flex-col justify-center items-center p-4">
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
    <div class="flex justify-center mb-4 space-x-6">
      <!-- Facebook Icon -->
      <a href="https://www.facebook.com" target="_blank" rel="noopener noreferrer" class="text-white hover:text-blue-500">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
          <path d="M22 12c0-5.5-4.5-10-10-10s-10 4.5-10 10c0 5 3.7 9.2 8.5 9.8v-6.9h-2.6v-2.6h2.6v-2c0-2.5 1.5-3.8 3.7-3.8 1.1 0 2.2.2 2.2.2v2.4h-1.2c-1.2 0-1.6.8-1.6 1.6v2.4h2.7l-1.5 2.6h-1.2v6.9c4.8-.6 8.5-4.8 8.5-9.8z"></path>
        </svg>
      </a>
      <!-- Instagram Icon -->
      <a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="text-white hover:text-pink-500">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
          <path d="M12 2.2c3.9 0 7 3.1 7 7s-3.1 7-7 7-7-3.1-7-7 3.1-7 7-7zm0-2.2c-5.1 0-9.2 4.2-9.2 9.2s4.1 9.2 9.2 9.2 9.2-4.2 9.2-9.2-4.1-9.2-9.2-9.2zm6.3 7.8c-.1 0-.2 0-.3.1-.3.1-.4.3-.4.6 0 .2.1.4.2.5.2.2.4.2.6.2.1 0 .3-.1.4-.1.2-.1.3-.2.4-.4 0-.2-.1-.3-.2-.5-.1-.2-.3-.2-.5-.2z"></path>
        </svg>
      </a>
      <!-- Twitter Icon -->
      <a href="https://www.twitter.com" target="_blank" rel="noopener noreferrer" class="text-white hover:text-blue-400">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
          <path d="M23.6 4.4c-.8.4-1.7.7-2.7.8 1-.6 1.7-1.5 2-2.6-.9.5-1.8.9-2.8 1.1-1.2-1.2-3.1-1.2-4.3 0-.8.8-1.1 1.9-.9 3-.7-.1-1.4-.3-2.1-.8-1.1-.8-1.7-2.1-1.4-3.4 1.2 1.4 2.8 2.1 4.5 2.2-1.2 1-2.8 1.5-4.4 1.5-3.4 0-6.4-3.1-6.4-6.9 0-.3 0-.6.1-.9-2.3 1.4-4 3.8-4 6.4 0 4.6 3.5 8.2 8 8.2 4.4 0 8.1-3.5 8.1-8.1 0-.1 0-.3 0-.4 1-.7 1.9-1.5 2.6-2.5z"></path>
        </svg>
      </a>
    </div>

    <!-- "jerrr" text -->
    <p class="text-sm mt-4">jerrr</p>
  </footer>
</template>

<style scoped>
/* Additional styling for the footer icons */
footer a {
  transition: color 0.3s ease;
}
</style>
