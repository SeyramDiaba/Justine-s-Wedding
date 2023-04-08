

<template>
  <nav class=" navbar sticky-top">
    <div class="container">
    <div class="navbar-logo">
      <img src="https://res.cloudinary.com/dcyay2pow/image/upload/v1680952005/favicon_a7l8ic.png" alt="Logo">
    </div>
    <button class="navbar-toggle" @click="toggleNav">
      <span></span>
      <span></span>
      <span></span>
    </button>
    <div class="navbar-links " :class="{ 'active': isNavOpen }">
      <ul>
        <li class="N900"><a  href="#whoWeAre">Bride & Groom</a></li>
        <li class="N900"><a href="#whenNwhere">When & Where</a></li>
        <li class="N900"><a href="#gallery">Gallery</a></li>
      </ul>
    </div>

    <div class="d-none d-md-block"></div>
  </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isNavOpen: false
    }
  },
  methods: {
    toggleNav() {
      this.isNavOpen = !this.isNavOpen;
    }
  }
}
</script>

<style>
a:hover {
  color: #b13a1a !important;
}
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: #d0edf5;
  box-shadow: 0px 2px 5px #b13a1a10;
}

.navbar-logo img {
  width: 70px;
  height: 50px;
}

.navbar-toggle {
  display: none;
  cursor: pointer;
  background: none;
  border: none;
}

.navbar-toggle span {
  display: block;
  width: 25px;
  height: 3px;
  margin-bottom: 5px;
  position: relative;
  background-color: #333;
  border-radius: 3px;
}

.navbar-links ul {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
}

.navbar-links li {
  margin: 0 1rem;
}

.navbar-links a {
  /* color: #333; */
  text-decoration: none;
  font-size: 1.2rem;
}

@media (max-width: 768px) {
  .navbar-toggle {
    display: block;
  }

  .navbar-links {
    position: absolute;
    top: 100%;
    left: 0;
    width: 100%;
    /* height: calc(100vh - 70); */
    background-color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.3s ease-in-out;
    z-index: 5;
  }

  .navbar-links.active {
    opacity: 1;
    visibility: visible;
  }

  .navbar-links ul {
    flex-direction: column;
  }

  .navbar-links li {
    margin: 1rem 0;
  }
}
</style> 
