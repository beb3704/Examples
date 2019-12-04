<template>
  <div>
    <nuxt />
  </div>
</template>

<style lang="scss">
@import '~assets/css/variables.scss';

*,
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
}

body {
  font-family: 'Lato', sans-serif;
  font-weight: 400;
  line-height: 1.7;
  color: color-primary;
  padding: 3rem;
  box-sizing: border-box;
}

.btn:link,
.btn:visited {
  text-transform: uppercase;
  text-decoration: none;
  padding: 1.5rem 4rem;
  display: inline-block;
  transition: all 0.2s;
  border-radius: 10rem;
  position: relative;
  font-size: 1.6rem;
}

.btn-white {
  background-color: #fff;
  color: $text-primary;
}

.btn:hover {
  transform: translateY(-0.3rem);
  box-shadow: 0 1rem 2rem;
}
.btn:active {
  transform: translateY(-0.1rem);
}

.btn::after {
  content: '';
  display: inline-block;
  height: 100%;
  width: 100%;
  border-radius: 10rem;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  transition: all 0.5s;
}

.btn-white::after {
  background-color: #fff;
}

.btn:hover::after {
  transform: scaleX(1.5) scaleY(1.4);

  opacity: 0;
}

.move-in-bottom {
  animation: moveInBottom 1s ease-out 0.75s;
  animation-fill-mode: backwards;
}

@keyframes moveInBottom {
  0% {
    opacity: 0;
    transform: translateY(3rem);
  }
  100% {
    opacity: 1;
    transform: translate(0);
  }
}
</style>
