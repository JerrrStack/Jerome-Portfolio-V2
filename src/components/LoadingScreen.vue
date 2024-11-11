<template>
  <div class="fixed inset-0 flex items-center justify-center bg-black z-50">
    <div class="relative flex items-center justify-center">
      <!-- Centered Logo with a Glow Effect and Pulse Animation -->
      <img src="@/assets/img/logo.png" alt="Logo" class="h-24 w-24 drop-shadow-glow animate-ping-slow" />
      <!-- Outer Dashed Border with Glow Effect and Pulse Animation -->
      <div class="absolute inset-0 border-gray-300 rounded-lg drop-shadow-glow animate-ping-slower"></div>
    </div>
  </div>
</template>

<style scoped>
/* Custom Ping Animation Speeds */
@keyframes ping-slow {
  0% {
    transform: scale(1);
    opacity: 1;
  }
  100% {
    transform: scale(1.2);
    opacity: 0;
  }
}
@keyframes ping-slower {
  0% {
    transform: scale(1);
    opacity: 1;
  }
  100% {
    transform: scale(1.3);
    opacity: 0;
  }
}

.animate-ping-slow {
  animation: ping-slow 2s ease-in-out infinite;
}
.animate-ping-slower {
  animation: ping-slower 3s ease-in-out infinite;
}

/* Glow Effect */
.drop-shadow-glow {
  filter: drop-shadow(0 0 8px rgba(255, 255, 255, 0.6));
}
</style>
