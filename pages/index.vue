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

    <!-- Services Section -->
    <section class="services-section">
      <div class="services-content">
        <h2 class="services-title">
          Efficiency Solutions for Modern Businesses
        </h2>
        <p class="services-description">
          Automate manual processes and streamline operations with our comprehensive digital solutions
        </p>

        <div class="services-grid">
          <!-- Web Applications -->
          <div class="service-card">
            <div class="service-icon">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M21 8V16C21 18.7614 18.7614 21 16 21H8C5.23858 21 3 18.7614 3 16V8C3 5.23858 5.23858 3 8 3H16C18.7614 3 21 5.23858 21 8Z" stroke="currentColor" stroke-width="2"/>
                <path d="M7 9L17 9" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <circle cx="9" cy="6" r="1" fill="currentColor"/>
                <circle cx="7" cy="6" r="1" fill="currentColor"/>
                <circle cx="11" cy="6" r="1" fill="currentColor"/>
              </svg>
            </div>
            <h3 class="service-title">Web Applications</h3>
            <p class="service-description">Custom web applications that streamline your business processes and improve team collaboration</p>
          </div>

          <!-- Automation Systems -->
          <div class="service-card">
            <div class="service-icon">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 3V7M12 17V21M4.22 4.22L6.34 6.34M17.66 17.66L19.78 19.78M1 12H5M19 12H23M4.22 19.78L6.34 17.66M17.66 6.34L19.78 4.22" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <circle cx="12" cy="12" r="3" stroke="currentColor" stroke-width="2"/>
              </svg>
            </div>
            <h3 class="service-title">Process Automation</h3>
            <p class="service-description">Eliminate repetitive tasks with intelligent automation systems that save time and reduce errors</p>
          </div>

          <!-- Professional Websites -->
          <div class="service-card">
            <div class="service-icon">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="2" y="4" width="20" height="16" rx="2" stroke="currentColor" stroke-width="2"/>
                <path d="M8 8H16M8 12H12" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <circle cx="6" cy="8" r="1" fill="currentColor"/>
                <circle cx="6" cy="12" r="1" fill="currentColor"/>
              </svg>
            </div>
            <h3 class="service-title">Professional Websites</h3>
            <p class="service-description">Modern, responsive websites that enhance your online presence and drive business growth</p>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="cta-section">
      <div class="cta-content">
        <h2 class="cta-title">
          Ready for powerful solutions?
        </h2>
        <p class="cta-description">
          Let's discuss your project and see how we can help bring your vision to life.
        </p>
        <div class="services-cta">
          <NuxtLink to="/contact" class="services-button">
            Transform Your Business
          </NuxtLink>
        </div>
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

@media (prefers-reduced-motion: reduce) {
  .wave, .pulse-glow, .highlight {
    animation: none;
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

.services-section {
  padding: 6rem 0 8rem;
  background: linear-gradient(180deg, #000 0%, #0a0a0a 100%);
  position: relative;
}

.services-content {
  max-width: 80rem;
  margin: 0 auto;
  padding: 0 1.5rem;
}

.services-title {
  font-size: 2.25rem;
  font-weight: bold;
  color: white;
  text-align: center;
  margin-bottom: 1rem;
}

@media (min-width: 768px) {
  .services-title {
    font-size: 3rem;
  }
}

.services-description {
  font-size: 1.25rem;
  color: #d1d5db;
  text-align: center;
  margin-bottom: 4rem;
  max-width: 48rem;
  margin-left: auto;
  margin-right: auto;
}

.services-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
  margin-bottom: 4rem;
}

@media (min-width: 768px) {
  .services-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
  }
}

@media (min-width: 1024px) {
  .services-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

.service-card {
  background: rgba(55, 65, 81, 0.15);
  backdrop-filter: blur(10px);
  padding: 2rem;
  border-radius: 1rem;
  text-align: center;
  transition: all 0.3s ease;
  border: 1px solid rgba(147, 51, 234, 0.1);
  position: relative;
  overflow: hidden;
}

.service-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(135deg, rgba(147, 51, 234, 0.05) 0%, transparent 50%);
  opacity: 0;
  transition: opacity 0.3s ease;
}

.service-card:hover {
  transform: translateY(-4px);
  border-color: rgba(147, 51, 234, 0.3);
  box-shadow: 0 20px 40px rgba(147, 51, 234, 0.1);
}

.service-card:hover::before {
  opacity: 1;
}

.service-icon {
  width: 4rem;
  height: 4rem;
  margin: 0 auto 1.5rem;
  color: #c4b5fd;
  transition: all 0.3s ease;
  position: relative;
  z-index: 1;
}

.service-card:hover .service-icon {
  color: #a855f7;
  transform: scale(1.1);
}

.service-icon svg {
  width: 100%;
  height: 100%;
}

.service-title {
  font-size: 1.5rem;
  font-weight: 600;
  color: white;
  margin-bottom: 1rem;
  position: relative;
  z-index: 1;
}

.service-description {
  font-size: 1rem;
  color: #9ca3af;
  line-height: 1.6;
  position: relative;
  z-index: 1;
}

.services-cta {
  text-align: center;
  margin-top: 3rem;
}

.services-button {
  display: inline-block;
  background: linear-gradient(135deg, #9333ea 0%, #7c3aed 100%);
  color: white;
  padding: 1rem 2.5rem;
  border-radius: 0.75rem;
  font-weight: 600;
  text-decoration: none;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(147, 51, 234, 0.3);
  position: relative;
  overflow: hidden;
}

.services-button::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
  transition: left 0.5s ease;
}

.services-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 25px rgba(147, 51, 234, 0.4);
}

.services-button:hover::before {
  left: 100%;
}

@media (prefers-reduced-motion: reduce) {
  .service-card,
  .services-button,
  .service-icon {
    transition: none;
    transform: none;
  }

  .service-card:hover,
  .services-button:hover {
    transform: none;
  }
}
</style>