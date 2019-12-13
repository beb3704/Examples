<template>
  <section class="section-about">
    <div class="row max-width">
      <div class="u-center-text margin-bottom-large">
        <h2 class="heading">Exciting tours for adventurous people</h2>
      </div>
      <div class="columns small-12 medium-6">
        <h3 class="heading-tertiary margin-bottom-small">
          You're going to fall in love with nature
        </h3>
        <p class="paragraph">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita
          dolorem dolores blanditiis error atque sequi ad sit recusandae,
          architecto consequuntur vel sed deserunt dignissimos laudantium iusto
          tempora illum saepe pariatur.
        </p>
        <h3 class="heading-tertiary margin-bottom-small">
          Live adventures like you never have before.
        </h3>
        <p class="paragraph">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita
          dolorem dolores blanditiis error atque sequi ad sit recusandae,
          architecto consequuntur vel sed deserunt dignissimos laudantium iusto
          tempora illum saepe pariatur. Lorem ipsum dolor sit amet consectetur,
          adipisicing elit. Nostrum neque ea tenetur odio commodi, vitae
          voluptas placeat molestias, quos totam doloremque. Officiis culpa amet
          delectus perferendis aspernatur voluptatem placeat ratione.
        </p>
        <nuxt-link to="/" class="btn-text">Learn more &rarr;</nuxt-link>
      </div>

      <div class="columns small-12 medium-6">
        <div class="composition">
          <img
            src="~assets/img/nat-1-large.jpg"
            class="composition__photo--1 composition__photo"
          />
          <img
            src="~assets/img/nat-2-large.jpg"
            class="composition__photo--2 composition__photo"
          />
          <img
            src="~assets/img/nat-3-large.jpg"
            class="composition__photo--3 composition__photo"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.composition {
  position: relative;
  &__photo {
    width: 55%;
    box-shadow: 0 1.5rem 4rem rgba($color-black, 0.4);
    border-radius: 2px;
    position: absolute;
    z-index: 10;
    transition: all 0.2s;
    outline-offset: 2rem;

    &--1 {
      left: 0;
      top: -2rem;
    }
    &--2 {
      right: 0;
      top: 2rem;
    }
    &--3 {
      left: 20%;
      top: 10rem;
    }

    &:hover {
      outline: 1.5rem solid $color-primary;
      transform: scale(1.05) translateY(-1rem);
      box-shadow: 0 2.5rem 4rem rgba($color-black, 0.5);
      z-index: 20;
    }
  }

  &:hover &__photo:not(:hover) {
    transform: scale(0.95);
  }
}

.section-about {
  background-color: $color-grey-light-1;
  padding: 25rem 0;
  margin-top: -10vh;
}
</style>
