<template>
  <div id="app" class="container">
    <navbar></navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
export default {
  name: 'app',
  components: {
    Navbar
  }
}
</script>

<style>
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

.container {
    max-width: 1200px;
    margin: 0 auto;
}
ul {
  padding: 0;
}

li {
  list-style-type: none;
}

a {
  text-decoration: none;
  color:#d0021b;
}

.button {
  color: #e6e6e6;
  background: #0a0a0a;
  border: none;
  font-size: 16px;
  border-radius: 3px;
  width: 200px;
  text-align: center;
  display: block;
  padding: 7px 0;
  margin: 10px auto;
}

.button:hover:enabled {
  background: linear-gradient(#1a1a1a,#0a0a0a);
  color: #fff;
  text-decoration: none;
}

.button:active {
  transform: translateY(1px);
}

.row {
  display: flex;
  justify-content: space-around;
}

.column {
  display: flex;
  flex-direction: column;
  width:500px;
  align-items: center;
}

.column input {
  border-radius: 3px;
  margin: 10px 0;
  padding: 5px;
  border: 1px solid rgba(0,0,0,0.43);
  font-size: 16px;
  width: 80%
}

.column textarea {
  border-radius: 3px;
  margin: 10px 0;
  padding: 5px;
  border: 1px solid rgba(0,0,0,0.43);
  font-size: 16px;
  width: 80%
}

.column label {
  text-align: center;
  font-size: 30px;
  font-weight: 200;
}

.header {
  text-align: center;
  font-size: 30px;
  font-weight: 2000;
}

.reset {
  border: none;
  background: transparent;
  color: #d0021b;
  display: block;
  width:100%;
  text-align: center;
}

.reset:hover {
  cursor: pointer;
}
</style>
