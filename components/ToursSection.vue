<template>
  <section class="Section">
    <div class="HeaderWrap">
      <h2 class="Header heading">Most Popular Tours</h2>
    </div>
    <div class="row expanded max-width">
      <div class="small-12 medium-4 columns">
        <div class="Card">
          <div class="Card-Side-Front Card-Side">lah blhalh fuck</div>
          <div class="Card-Side-Back Card-Side Card-Side-Back-Orange">
            lah blhaasdfasdflh fuck
          </div>
        </div>
      </div>
      <div class="small-12 medium-4 columns">2</div>
      <div class="small-12 medium-4 columns">3</div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.Section {
  background-color: $color-grey-light-1;
  padding: 35rem 0 50rem 0;
  margin-top: -15rem;
}
.HeaderWrap {
  text-align: center;
}
.Card {
  perspective: 150rem;
  -moz-perspective: 150rem;
  margin: 5rem;
  position: relative;
  height: 50rem;

  &-Side {
    color: white;
    font-size: 2rem;
    height: 50rem;
    transition: all 0.8s ease;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    backface-visibility: hidden;
    box-shadow: 0 1.5rem 4rem rgba($color-black, 0.15);
    &-Front {
      background-color: $color-white;
    }
    &-Back {
      transform: rotateY(180deg);
      &-Orange {
        background-image: linear-gradient(
          to right bottom,
          $color-secondary-light,
          $color-secondary-dark
        );
      }
    }
  }

  &:hover &-Side-Front {
    transform: rotateY(-180deg);
  }
  &:hover &-Side-Back {
    transform: rotateY(0deg);
  }
}
</style>
