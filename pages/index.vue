<template>
  <div>
    <!-- Hero Section -->
    <section class="hero-section">
      <div class="wave-container">
        <div class="wave"></div>
        <div class="wave"></div>
        <div class="wave"></div>
        <div class="wave"></div>
        <div class="pulse-glow"></div>
        <div class="floating-particles">
          <div class="particle"></div>
          <div class="particle"></div>
          <div class="particle"></div>
        </div>
      </div>

      <div class="content">
        <div class="badge">
          Now accepting projects for Q4 2025
        </div>

        <h1 class="title">
          Strengthen your company with
          <span class="highlight">powerful solutions</span>
        </h1>

        <p class="description">
          We create powerful solutions to your needs.
          From websites to full applications, we bring your vision to life.
        </p>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="cta-section">
      <div class="cta-content">
        <h2 class="cta-title">
          Ready to transform your digital presence?
        </h2>
        <p class="cta-description">
          Let's discuss your project and see how we can help bring your vision to life.
        </p>
        <NuxtLink
            to="/contact"
            class="cta-button"
        >
          Start Your Project
        </NuxtLink>
      </div>
    </section>
  </div>
</template>

<script setup>
useSeoMeta({
  title: 'Khode',
  ogTitle: 'Khode',
  description: 'Strengthen your company with powerful solutions.',
  ogDescription: 'Strengthen your company with powerful solutions.',
})
</script>

<style scoped>
.hero-section {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  background: linear-gradient(180deg, #000 0%, #0a0a0a 70%, #050505 100%);
  overflow: hidden;
}

.wave-container {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 0.7;
  z-index: 1;
}

.wave {
  position: absolute;
  width: 120%;
  height: 120%;
  background: radial-gradient(
      ellipse at center,
      rgba(147, 51, 234, 0.4) 0%,
      rgba(147, 51, 234, 0.2) 25%,
      rgba(147, 51, 234, 0.1) 50%,
      rgba(59, 130, 246, 0.05) 75%,
      transparent 100%
  );
  border-radius: 50%;
  filter: blur(40px);
  animation: waveFloat 1s ease-in-out infinite;
}

.wave:nth-child(1) {
  top: -90%;
  left: -30%;
  animation-delay: 0s;
  animation-duration: 15s;
  background: radial-gradient(
      ellipse at center,
      rgba(147, 51, 234, 0.5) 0%,
      rgba(147, 51, 234, 0.2) 40%,
      transparent 80%
  );
}

.wave:nth-child(2) {
  top: -10%;
  right: -30%;
  animation-delay: -2s;
  animation-duration: 18s;
  opacity: 0.6;
  background: radial-gradient(
      ellipse at center,
      rgba(0, 60, 142, 0.4) 0%,
      rgba(7, 36, 83, 0.3) 40%,
      transparent 80%
  );
}

.wave:nth-child(3) {
  bottom: -30%;
  left: -20%;
  animation-delay: -4s;
  animation-duration: 10s;
  opacity: 0.5;
  background: radial-gradient(
      ellipse at center,
      rgba(168, 85, 247, 0.3) 0%,
      rgba(168, 85, 247, 0.1) 50%,
      transparent 80%
  );
}

.wave:nth-child(4) {
  top: 90%;
  left: 50%;
  animation-delay: -6s;
  animation-duration: 7s;
  opacity: 0.4;
  transform-origin: center;
  background: radial-gradient(
      ellipse at center,
      rgba(147, 51, 234, 0.3) 0%,
      rgba(147, 51, 234, 0.1) 60%,
      transparent 90%
  );
}

.wave:nth-child(5) {
  top: 20%;
  right: -10%;
  animation-delay: -3s;
  animation-duration: 9s;
  opacity: 0.3;
  width: 80%;
  height: 80%;
  background: radial-gradient(
      ellipse at center,
      rgba(34, 197, 94, 0.2) 0%,
      rgba(34, 197, 94, 0.05) 50%,
      transparent 80%
  );
}

.wave:nth-child(6) {
  bottom: 10%;
  right: 20%;
  animation-delay: -5s;
  animation-duration: 11s;
  opacity: 0.35;
  width: 90%;
  height: 90%;
  background: radial-gradient(
      ellipse at center,
      rgba(236, 72, 153, 0.25) 0%,
      rgba(236, 72, 153, 0.08) 50%,
      transparent 80%
  );
}

.pulse-glow {
  position: absolute;
  top: 10%;
  left: 20%;
  width: 60%;
  height: 40%;
  background: radial-gradient(
      circle,
      rgba(147, 51, 234, 0.15) 0%,
      rgba(147, 51, 234, 0.08) 40%,
      rgba(59, 130, 246, 0.05) 70%,
      transparent 100%
  );
  border-radius: 50%;
  filter: blur(80px);
  animation: pulseGlow 5s ease-in-out infinite;
  z-index: 0;
}

@keyframes waveFloat {
  0%, 100% {
    transform: translate(0px, 0px) rotate(0deg) scale(1);
  }
  20% {
    transform: translate(-40px, -60px) rotate(8deg) scale(1.08);
  }
  40% {
    transform: translate(60px, -30px) rotate(-5deg) scale(0.92);
  }
  60% {
    transform: translate(-25px, 45px) rotate(3deg) scale(1.05);
  }
  80% {
    transform: translate(35px, -15px) rotate(-2deg) scale(0.98);
  }
}

@keyframes pulseGlow {
  0%, 100% {
    opacity: 0.4;
    transform: scale(1) rotate(0deg);
  }
  25% {
    opacity: 0.7;
    transform: scale(1.15) rotate(2deg);
  }
  50% {
    opacity: 0.8;
    transform: scale(1.2) rotate(-1deg);
  }
  75% {
    opacity: 0.6;
    transform: scale(1.1) rotate(1.5deg);
  }
}

@keyframes particleFloat {
  0%, 100% {
    transform: translate(0px, 0px) scale(1);
    opacity: 0.3;
  }
  25% {
    transform: translate(-100px, -150px) scale(1.2);
    opacity: 0.8;
  }
  50% {
    transform: translate(120px, -80px) scale(0.8);
    opacity: 0.5;
  }
  75% {
    transform: translate(-80px, 100px) scale(1.1);
    opacity: 0.7;
  }
}

.content {
  position: relative;
  z-index: 10;
  width: 100%;
  padding: 0 1.5rem 0 2rem;
}

@media (min-width: 768px) {
  .content {
    padding-left: 4rem;
  }
}

.badge {
  display: inline-block;
  padding: 0.25rem 0.75rem;
  background: rgba(31, 41, 55, 0.8);
  color: #d1d5db;
  border-radius: 9999px;
  font-size: 0.75rem;
  margin-bottom: 1rem;
  backdrop-filter: blur(15px);
  border: 1px solid rgba(147, 51, 234, 0.3);
  box-shadow: 0 4px 6px rgba(147, 51, 234, 0.1);
}

.title {
  font-size: 1.875rem;
  font-weight: bold;
  color: white;
  margin-bottom: 1rem;
  line-height: 1.2;
  max-width: 64rem;
}

@media (min-width: 768px) {
  .title {
    font-size: 3rem;
  }
}

.highlight {
  color: #c4b5fd;
  text-shadow: 0 0 30px rgba(147, 51, 234, 0.6);
  animation: textGlow 4s ease-in-out infinite alternate;
}

@keyframes textGlow {
  from {
    text-shadow: 0 0 20px rgba(147, 51, 234, 0.5);
  }
  to {
    text-shadow: 0 0 40px rgba(147, 51, 234, 0.8);
  }
}

.description {
  font-size: 1rem;
  color: #9ca3af;
  margin-bottom: 1.5rem;
  max-width: 32rem;
  line-height: 1.6;
}

@media (min-width: 768px) {
  .description {
    font-size: 1.125rem;
  }
}

.cta-section {
  padding: 6rem 0;
  background: #000;
  position: relative;
}

.cta-content {
  max-width: 64rem;
  margin: 0 auto;
  padding: 0 1.5rem;
  text-align: center;
}

.cta-title {
  font-size: 2.25rem;
  font-weight: bold;
  color: white;
  margin-bottom: 1.5rem;
}

.cta-description {
  font-size: 1.25rem;
  color: #d1d5db;
  margin-bottom: 2rem;
}

.cta-button {
  display: inline-block;
  background: white;
  color: #111827;
  padding: 1rem 2rem;
  border-radius: 0.5rem;
  font-weight: 600;
  text-decoration: none;
  transition: all 0.3s ease;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.cta-button:hover {
  background: #f3f4f6;
  transform: translateY(-2px);
  box-shadow: 0 8px 12px rgba(0, 0, 0, 0.15);
}
</style>