<template>
  <div class="containerr" :class="{'shrink': showNav}" @click="showNav = !showNav">
    <div>
      <Logo />
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showNav: true
    }
  }
}
</script>

<style scoped>
.containerr {
  width: 100vw;
  min-height: 100vh;

  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;

  position: absolute;
  top: 0;
  background: #fff;
  transition: .3s all ease-in-out;

  border-radius: 6px;
  cursor: pointer;
  overflow: hidden;

}

.shrink {
  transform: scale(.9) translateX(250px);
  overflow: hidden;
  box-shadow: -5px 5px 20px #333;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
