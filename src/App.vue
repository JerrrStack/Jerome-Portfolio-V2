<script>
import { ref, onMounted } from "vue";
import LoadingScreen from "./components/LoadingScreen.vue";
import MainPage from "./components/MainPage.vue";
import '@fortawesome/fontawesome-free/css/all.min.css';
// Importing fonts globally
import '@fontsource/poppins';  // Default weight
import '@fontsource/roboto';    // Default weight



export default {
  components: {
    LoadingScreen,
    MainPage,
  },
  setup() {
    const loading = ref(true);

    onMounted(() => {
      setTimeout(() => {
        loading.value = false;
      }, 3000); // Display loading screen for 3 seconds
    });

    return { loading };
  },
};
</script>

<template>
  <div>
    <LoadingScreen v-if="loading" />
    <MainPage v-else />

    <MainPage />
  </div>
</template>
