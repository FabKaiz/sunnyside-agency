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
      <div class="services-text">
        <h2>Graphic Design</h2>
        <p>
          Great design makes you memorable. We deliver artwork that underscores
          your brand message and captures potential clients’ attention.
        </p>
      </div>
    </div>
    <div class="service-image-and-info service-photography">
      <div class="services-text">
        <h2>Photography</h2>
        <p>
          Increase your credibility by getting the most stunning, high-quality
          photos that improve your business image.
        </p>
      </div>
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
  grid-template-rows: 1fr 1fr 1fr;
  gap: 0px 0px;
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

.service-graphic {
  background: url(../assets/images/desktop/image-graphic-design.jpg);
  width: 100%;
  height: auto;
  color: #25564b;
}

.service-photography {
  background: url(../assets/images/desktop/image-photography.jpg);
  width: 100%;
  height: auto;
  color: #19536b;
}

.service-image-and-info {
  background-size: cover;
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  justify-content: end;
}

.services-text {
  margin: 3rem auto;
  max-width: 340px;

  h2 {
    margin: 0;
    font-size: 1.8rem;
    font-weight: 900;
  }

  p {
    margin: 1.5rem 0 0;
    text-align: center;
    line-height: 1.6em;
    font-size: 16px;
  }
}
</style>
