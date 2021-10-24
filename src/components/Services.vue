<!-- @format -->

<template>
  <div class="services-grid">
    <div class="services-info service-left">
      <h2>Transform your brand</h2>
      <p>
        We are a full-service creative agency specializing in helping brands
        grow fast. Engage your clients through compelling visuals that do most
        of the marketing for you.
      </p>
      <button class="learn-more btn-yellow">LEARN MORE</button>
    </div>

    <img
      class="services-image service-right"
      src="../assets/images/desktop/image-transform.jpg"
      alt="egg picture"
    />
    <img
      class="services-image"
      src="../assets/images/desktop/image-stand-out.jpg"
      alt="glass picture"
    />

    <div class="services-info">
      <h2>Stand out to the right audience</h2>
      <p>
        Using a collaborative formula of designers, researchers, photographers,
        videographers, and copywriters, we’ll build and extend your brand in
        digital places.
      </p>
      <button class="learn-more btn-pink">LEARN MORE</button>
    </div>
    <div class="service-image-and-info service-graphic">
      <h2>Graphic Design</h2>
      <p>
        Great design makes you memorable. We deliver artwork that underscores
        your brand message and captures potential clients’ attention.
      </p>
    </div>
    <div class="service-image-and-info service-photography">
      <h2>Photography</h2>
      <p>
        Great design makes you memorable. We deliver artwork that underscores
        your brand message and captures potential clients’ attention.
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.services-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: repeat(3);
}

.services-info {
  margin: auto;
  max-width: 330px;

  h2 {
    font-size: 2.25rem;
    font-weight: 900;
    color: #23303e;
  }

  p {
    margin: 1.4rem 0;
    color: #818498;
    line-height: 1.6em;
  }

  button {
    font-weight: 900;
    color: #23303e;
    letter-spacing: 0.1em;
    font-size: 16px;
    border: none;
    background: none;
    position: relative;
    cursor: pointer;

    &::after {
      content: '';
      position: absolute;
      z-index: -1;
      bottom: -1px;
      left: -1px;
      right: -1px;
      height: 8px;
      border-radius: 4px;
      opacity: 0.25;
      transition: all 0.1s linear;
    }

    &:hover::after {
      opacity: 1;
    }
  }

  .btn-yellow::after {
    background: #fad400;
  }

  .btn-pink::after {
    background: #fe7867;
  }
}

.services-image {
  width: 100%;
  height: auto;
}

.service-right {
  grid-row: 1/2;
  grid-column: 2/3;
}

.service-left {
  margin: auto;
  grid-row: 1/2;
  grid-column: 1/2;
}
</style>
