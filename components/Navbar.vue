<template>
  <div class="navigation">
    <ul>
      <li><nuxt-link to="/">start</nuxt-link></li>
      <li><nuxt-link to="/about">about</nuxt-link></li>
      <li><nuxt-link to="/uses">uses</nuxt-link></li>
      <li><nuxt-link to="/blog">blog</nuxt-link></li>
      <li><nuxt-link to="/policy">policy</nuxt-link></li>
    </ul>
  </div>
</template>

<style scoped>
  .navigation {
    width: 100vw;
    min-height: 100vh;
    padding: 16px;
    background: #0b8457;
  }
  ul {
    list-style: none;
  }
  li {
    margin-bottom: 16px;
    text-transform: uppercase;
  }
  a {
    color: #fefefe;
    text-decoration: none;
  }
</style>