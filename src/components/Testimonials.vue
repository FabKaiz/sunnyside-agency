<template>
  <div class="testimonials">
    <h3>Client Testimonials</h3>
    <div class="testimonials-container">
      <div class="testimonial-card">
        <img src="../assets/images/image-emily.jpg" alt="Picture of a client" />
        <p class="description">
          We put our trust in Sunnyside and they delivered, making sure our
          needs were met and deadlines were always hit.
        </p>
        <div>
          <p class="name">Emily R.</p>
          <p class="job">Marketing Director</p>
        </div>
      </div>
      <div class="testimonial-card">
        <img
          src="../assets/images/image-thomas.jpg"
          alt="Picture of a client"
        />
        <p class="description">
          Sunnyside’s enthusiasm coupled with their keen interest in our brand’s
          success made it a satisfying and enjoyable experience.
        </p>
        <div>
          <p class="name">Thomas S.</p>
          <p class="job">Chief Operating Officer</p>
        </div>
      </div>
      <div class="testimonial-card">
        <img
          src="../assets/images/image-jennie.jpg"
          alt="Picture of a client"
        />
        <p class="description">
          Incredible end result! Our sales increased over 400% when we worked
          with Sunnyside. Highly recommended!
        </p>
        <div>
          <p class="name">Jennie F.</p>
          <p class="job">Business Owner</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.testimonials {
  padding: 120px 0 80px;

  h3 {
    text-align: center;
    text-transform: uppercase;
    font-size: 21px;
    font-family: 'Fraunces', serif;
    letter-spacing: 0.25em;
    color: #a7abae;
    margin: 0;
  }
}

.testimonials-container {
  display: flex;
  justify-content: space-between;
  max-width: 1100px;
  margin: 0 auto;
}

.testimonial-card {
  max-width: 350px;
  margin: 4rem 0;
  text-align: center;

  img {
    border-radius: 99%;
    width: 70px;
  }

  p {
    margin: 0;
  }

  .description {
    margin: 4rem 0;
    line-height: 1.6em;
    color: #5a636c;
  }

  .name {
    font-family: 'Fraunces', serif;
    font-weight: 900;
    color: #23303e;
  }

  .job {
    font-size: 14px;
    margin: 12px;
    color: #a7abae;
  }
}
</style>
