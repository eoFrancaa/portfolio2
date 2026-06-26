<script setup>

</script>

<template>
    <header>
        <nav>
            <ul>
              <li>  <router-link to="/" class="nav-link active"> Home</router-link></li>
                <li><router-link to="/about" class="nav-link">About</router-link></li>
                <li><router-link to="/projects" class="nav-link">Projects</router-link></li>
                <li><router-link to="/connect" class="nav-link">Connect</router-link></li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  display: flex;
  justify-content: center;
  padding: 15px 0;
  z-index: 100;
  background-color: rgba(240, 240, 240, 0.75);
  backdrop-filter: blur(10px);
}

header nav ul {
  display: flex;
  gap: 10px;
  padding: 6px 12px;
  border-radius: 50px;
  border: 2px solid #ddd;
  background-color: #fff;
  list-style: none;
}

header nav ul li a {
  display: block;
  padding: 8px 16px;
  border-radius: 50px;
  font-size: 0.9rem;
  color: #333;
  text-decoration: none;
  transition: 0.3s;
}

header nav ul li a.router-link-exact-active {
  background-color: #111;
  color: #fff;
}

header nav ul li a:hover:not(.active) {
  background-color: #eee;
}
</style>
