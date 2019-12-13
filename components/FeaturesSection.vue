<template>
  <section class="Section">
    <div class="row expanded max-width">
      <div class="columns small-12 medium-6 large-3">
        <div class="BoxArea">
          <i class="icon-basic-world icon-size"></i>
          <h3 class="heading margin-bottom-small">A Header</h3>
          <p class="feature-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat
            incidunt, sequi ipsam, distinctio aliquam, aperiam corrupti
            reprehenderit exercitationem velit officiis modi dolores accusantium
          </p>
        </div>
      </div>
      <div class="columns small-12 medium-6 large-3">
        <div class="BoxArea">
          <i class="icon-basic-compass icon-size"></i>
          <h3 class="heading margin-bottom-small">A Header</h3>
          <p class="feature-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat
            incidunt, sequi ipsam, distinctio aliquam, aperiam corrupti
            reprehenderit exercitationem velit officiis modi dolores accusantium
          </p>
        </div>
      </div>
      <div class="columns small-12 medium-6 large-3">
        <div class="BoxArea">
          <i class="icon-basic-map icon-size"></i>
          <h3 class="heading margin-bottom-small">A Header</h3>
          <p class="feature-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat
            incidunt, sequi ipsam, distinctio aliquam, aperiam corrupti
            reprehenderit exercitationem velit officiis modi dolores accusantium
          </p>
        </div>
      </div>
      <div class="columns small-12 medium-6 large-3">
        <div class="BoxArea">
          <i class="icon-basic-heart icon-size"></i>
          <h3 class="heading margin-bottom-small">A Header</h3>
          <p class="feature-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat
            incidunt, sequi ipsam, distinctio aliquam, aperiam corrupti
            reprehenderit exercitationem velit officiis modi dolores accusantium
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.icon-size {
  font-size: 6rem;
  display: inline-block;
  background-image: linear-gradient(
    to right,
    $color-primary-light,
    $color-primary-dark
  );
  background-clip: text;
  color: transparent;
}
.Section {
  padding: 20rem 0;
  background-image: linear-gradient(
      to right bottom,
      rgba($color-primary-light, 0.8),
      rgba($color-primary-dark, 0.8)
    ),
    url('~assets/img/nat-4.jpg');
  background-size: cover;
  transform: skewY(-7deg);
  margin-top: -15rem;

  & > * {
    transform: skewY(7deg);
  }
}
.BoxArea {
  background-color: rgba($color-white, 0.8);
  font-size: 1.5rem;
  padding: 2.5rem;
  text-align: center;
  border-radius: 3px;
  box-shadow: 0 1.5rem 4rem rgba($color: $color-black, $alpha: 0.15);
  transition: transform 0.3s;
  margin: 3rem;

  &:hover {
    transform: translateY(-1.5rem) scale(1.03);
  }
}
.heading {
}
</style>
