<template>
  <section id="main">
    <div class="relative flex flex-col lg:flex-row h-auto lg:h-screen">
      <!-- Right Section (Introduction and About Me Button) -->
      <div
        class="w-full lg:w-1/2 h-auto bg-black flex flex-col justify-center items-center p-4 text-center text-white"
      >
        <div :class="{ 'animate-fadeUp': isVisible }">
          <h1 class="text-3xl md:text-5xl font-bold mb-4 font-mono">
            Hi! I'm Jerome Bernal
          </h1>
          <p class="text-lg md:text-2xl mb-10 font-bold font-mono">
            Software Engineer
          </p>
        </div>

        <!-- About Me Button -->
        <button
          class="mt-8 px-6 py-3 bg-gray-700 text-white rounded-md hover:bg-gray-600"
          @click="scrollToAbout"
        >
          About Me
        </button>
      </div>

      <!-- Left Section (Image) -->
      <div
        class="w-full lg:w-1/2 h-auto bg-black flex flex-col justify-center items-center p-4"
      >
        <div
          class="mt-8 lg:mt-0 flex justify-center"
          :class="{ 'animate-fadeRight': isVisible }"
        >
          <img
            alt="John Jerome Bernal"
            src="@/assets/img/jerrr.png"
            class="object-cover max-w-full h-auto"
          />
        </div>
      </div>
    </div>
  </section>

  <!-- <section class="bg-gray-900 text-white py-16 px-6" id="download-cv">
    <div class="max-w-4xl mx-auto text-center">
      <h2 class="text-3xl md:text-5xl font-bold mb-6">Download My CV</h2>
      <p class="text-lg md:text-xl mb-8">
        Interested in learning more about my experience and skills? Download my CV and let’s connect!
      </p>
      <a
        href="@/assets/pdf/my_resume.pdf"
        download
        class="inline-block px-8 py-4 bg-blue-600 text-white font-medium text-lg rounded-md shadow-md hover:bg-blue-500 transition duration-300"
      >
        Download CV
      </a>
    </div>
  </section> -->

  <!-- About Me Section -->
  <section id="about" class="bg-white py-16 px-4 md:px-16">
    <div class="max-w-7xl mx-auto text-center">
      <h2 class="text-4xl font-semibold text-gray-800 mb-6">About Me</h2>
      <p class="text-lg text-gray-600 mb-4">
        I’m a software engineer with almost four years of experience in designing, developing, and maintaining software solutions.I’ve worked on various projects, collaborating with skilled teams and continuously learning new technologies
      </p>
      <p class="text-lg text-gray-600">
        For my past time, my hobbies include working out, jogging, and playing badminton. I enjoy staying active and challenging myself toimprove in each of these activities
      </p>
    </div>
  </section>

  <footer class="text-center py-8 bg-gray-800 text-white">
    <!-- Social Media Links -->
    <div class="flex justify-center mb-6 space-x-8">
      <!-- Facebook Icon -->
      <a
        href="https://www.facebook.com/JJbernal07"
        target="_blank"
        rel="noopener noreferrer"
        class="text-blue-500 border-2 border-blue-500 p-3 rounded-full hover:text-white hover:border-white"
      >
        <i class="fab fa-facebook-f text-2xl"></i>
      </a>
      <!-- Instagram Icon -->
      <a
        href="https://www.instagram.com/jerrrrr04"
        target="_blank"
        rel="noopener noreferrer"
        class="text-pink-500 border-2 border-pink-500 p-3 rounded-full hover:text-white hover:border-white"
      >
        <i class="fab fa-instagram text-2xl"></i>
      </a>
      <!-- LinkedIn Icon -->
      <a
        href="https://www.linkedin.com/in/john-jerome-bernal-561821212/"
        target="_blank"
        rel="noopener noreferrer"
        class="text-blue-700 border-2 border-blue-700 p-3 rounded-full hover:text-white hover:border-white"
      >
        <i class="fab fa-linkedin-in text-2xl"></i>
      </a>
    </div>

    <!-- Copyright Section -->
    <div class="text-sm">
      <p>&copy; 2024 My Personal Website v2, made with Vue js.</p>
    </div>

    <!-- Footer "jerrr" Text -->
    <p @click="scrollToMain" class="text-2xl mt-4 font-semibold text-transparent bg-clip-text bg-gradient-to-r from-pink-500 to-purple-600 hover:text-white transition-all duration-300 cursor-pointer">
    Jerrr
  </p>
  </footer>
</template>

<style scoped>
/* Additional styling for the footer icons */
footer a {
  transition: color 0.3s ease;
}
</style>

<script>
export default {
  data() {
    return {
      isVisible: false, // Controls animation visibility
    };
  },
  mounted() {
    // Trigger animations on page load
    this.isVisible = true;
  },
  methods: {
    scrollToAbout() {
      document.getElementById("about").scrollIntoView({ behavior: "smooth" });
    },
    scrollToMain() {
      document.getElementById("main").scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>
