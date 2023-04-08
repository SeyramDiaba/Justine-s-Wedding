<template>
    <div class="countdown">
      <!-- <h2>Countdown to April 22nd, 2023</h2> -->
      <div class="timer">
        <div class="timer-item mx-lg-10 mx-5">
          <div class="timer-value N900">{{ days }}</div>
          <div class="timer-label N900">Days</div>
        </div>
        <div class="timer-item mx-lg-10 mx-5">
          <div class="timer-value N900">{{ hours }}</div>
          <div class="timer-label N900">Hours</div>
        </div>
        <div class="timer-item mx-lg-10 mx-5">
          <div class="timer-value N900">{{ minutes }}</div>
          <div class="timer-label N900">Minutes</div>
        </div>
        <div class="timer-item mx-lg-10 mx-5">
          <div class="timer-value N900">{{ seconds }}</div>
          <div class="timer-label N900">Seconds</div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue';
  
  export default {
    setup() {
      const countdownDate = new Date('April 15, 2023 00:00:00').getTime();
      const now = new Date().getTime();
      const timeLeft = countdownDate - now;
  
      const days = ref(Math.floor(timeLeft / (1000 * 60 * 60 * 24)));
      const hours = ref(
        Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60))
      );
      const minutes = ref(Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60)));
      const seconds = ref(Math.floor((timeLeft % (1000 * 60)) / 1000));
  
      setInterval(() => {
        const now = new Date().getTime();
        const timeLeft = countdownDate - now;
        days.value = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
        hours.value = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        minutes.value = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
        seconds.value = Math.floor((timeLeft % (1000 * 60)) / 1000);
      }, 1000);
  
      return { days, hours, minutes, seconds };
    },
  };
  </script>
  
  <style>
  .countdown {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
  }
  
  .timer {
    display: flex;
    justify-content: space-between;
    margin-top: 1rem;
  }
  
  .timer-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    font-size: 1.5rem;
    font-weight: bold;
    text-transform: uppercase;
  }
  
  .timer-value {
    font-size: 2.5rem;
    font-weight: bold;
  }
  
  .timer-label {
    margin-top: 0.5rem;
    font-size: 0.75rem;
    font-weight: normal;
    text-transform: uppercase;
  }
  </style>
  