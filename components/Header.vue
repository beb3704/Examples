<template>
  <div>
    <header class="header">
      <div class="header__logo-box">
        <img
          src="~assets/img/logo-white.png"
          alt="CrownLogo"
          class="header__logo"
        />
      </div>
      <div class="header__text-box">
        <h1 class="header__primary">
          <span class="header__primary-main">Outdoors</span>
          <span class="header__primary-sub">is where life happens</span>
        </h1>
        <a href="#" class="btn btn-white move-in-bottom">Discover our Tours</a>
      </div>
    </header>

    <svg width="0" height="0" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <clipPath id="svgClipPath" clipPathUnits="objectBoundingBox">
          <polygon points="0, 0,1, 0, 1, .92, 0, 1" />
        </clipPath>
        <use clip-path="url(#svgClipPath)" />
      </defs>
    </svg>
  </div>
</template>
<style scoped lang="scss">
.header {
  height: 95vh;
  background-image: linear-gradient(
      to right bottom,
      rgba($color-primary-light, 0.8),
      rgba($color-primary-dark, 0.8)
    ),
    url('~assets/img/hero.jpg');
  background-size: cover;
  background-position: top;
  clip-path: url(#svgClipPath);
  position: relative;

  &__logo {
    height: 3.5rem;

    &-box {
      position: absolute;
      top: 4rem;
      left: 4rem;
    }
  }

  &__text-box {
    position: absolute;
    top: 43%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }

  &__primary {
    text-transform: uppercase;
    color: $color-white;
    backface-visibility: hidden;
    margin-bottom: 6rem;

    &-main {
      display: block;
      font-weight: 400;
      font-size: 6rem;
      letter-spacing: 3.5rem;

      animation-name: moveInLeft;
      animation-duration: 2s;
      animation-timing-function: ease-out;
    }

    &-sub {
      display: block;
      font-size: 2rem;
      font-weight: 700;
      letter-spacing: 1.7rem;
      margin-left: -1.2rem;
      animation: moveInRight 2s ease-out;
    }
  }
}

//KeyFrames
@keyframes moveInLeft {
  0% {
    opacity: 0;
    transform: translateX(-10rem);
  }
  80% {
    transform: translate(1rem);
  }
  100% {
    opacity: 1;
    transform: translate(0);
  }
}

@keyframes moveInRight {
  0% {
    opacity: 0;
    transform: translateX(10rem);
  }
  70% {
    transform: translate(-0.1rem);
  }
  100% {
    opacity: 1;
    transform: translate(0);
  }
}
</style>
