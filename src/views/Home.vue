<template>
  <div class="contentSpace">
    <section id="hero">
      <div class="pitch">
        <h1>A creative meetup</h1>
        <h3>We are calling out for Visual, UI/UX, and Interaction Design enthusiasts in the Trento community</h3>
        <div class="cta">
          <button>
            <a
              href="https://www.eventbrite.com/e/specktech-retreat-v2-tickets-67052270145"
              target="_blank"
            >Join meetup</a>
          </button>
          <span>Go on, it's free!</span>
        </div>
      </div>
      <div class="illustration">
        <img src="../assets/illustration_01_welcome.png" alt="Welcome" />
      </div>
    </section>

    <section id="whoWeAre">
      <div class="illustration">
        <img src="../assets/illustration_02_who we are.png" alt="Who we are" />
      </div>
      <div class="pitch">
        <h2>We are the design freaks.</h2>
        <p
          class="body-section"
        >We provide an opportunity for design students in Trento to exchange ideas, learn new skills and have fun while meeting new exciting creative minds.</p>
        <div class="grid-interests">
          <div class="interest">
            <img src="../assets/icons_02_uiux.png" alt="UI and UX" />
            <p class="caption">UI/UX</p>
          </div>
          <div class="interest">
            <img src="../assets/icons_02_visualDesign.png" alt="Visual Design" />
            <p class="caption">visual design</p>
          </div>
          <div class="interest">
            <img src="../assets/icons_02_webDesign.png" alt="Web Design" />
            <p class="caption">web design</p>
          </div>
          <div class="interest">
            <img src="../assets/icons_02_illustration.png" alt="Illustration" />
            <p class="caption">illustration</p>
          </div>
          <div class="interest">
            <img src="../assets/icons_02_photogrphy.png" alt="Photography" />
            <p class="caption">photography</p>
          </div>
          <div class="interest">
            <img src="../assets/icons_02_marketing.png" alt="Marketing" />
            <p class="caption">marketing</p>
          </div>
        </div>
      </div>
    </section>

    <section id="joinUs">
      <div class="pitch">
        <h2>Do more of what you love, with us</h2>
        <p
          class="body-section"
        >Events include talks from guest speakers on topics around design, photography and professional arts, networking opportunities, dynamic workshop and a good old-fashioned chin-wag over a beer or two.</p>
        <div class="cta">
          <button>
            <a
              href="https://www.eventbrite.com/e/specktech-retreat-v2-tickets-67052270145"
            >Join meetup</a>
          </button>
          <span>Go on, it's free!</span>
        </div>
      </div>
      <div class="illustration">
        <img src="../assets/illustration_03_what we do.png" alt="What we do" />
      </div>
    </section>

    <section id="social">
      <div class="illustration">
        <img src="../assets/illustration_05_feedback.png" alt="Share your ideas" />
      </div>
      <div class="pitch">
        <h2>Got an idea? Share it!</h2>
        <p class="body-section">
          Our community listen to new and old members alike.
          <br />If you have an idea, a suggestion or a feature request, please let us know! You can find us litterally everywhere.
        </p>
        <div class="social-link">
          <a class="link" href="https://www.facebook.com/designfreaksclub/" target="_blank">
            <img src="../assets/icon_05_facebook.png" alt="Facebook" />
            <p>Facebook</p>
          </a>
          <a class="link" href="https://www.instagram.com/designfreaksclub/?hl=it" target="_blank">
            <img src="../assets/icon_05_instagram.png" alt="Instagram" />
            <p>Instagram</p>
          </a>
          <a class="link" href="#">
            <img src="../assets/icon_05_telegram.png" alt="Telegram" />
            <p>Telegram</p>
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style lang="scss">
.grid-interests {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(2, 1fr);
  text-align: center;
  padding: 3rem 0 0 0;
  font-size: 12px;
}

.social-link {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  padding: 2rem 0 0 1rem;
}

@media screen and (min-width: 768px) {
  section {
    grid-template-columns: repeat(12, 1fr);
    grid-template-rows: 100%;
  }

  #hero {
    padding: 8rem 0rem 2rem 0rem;
    .pitch {
      grid-column: 1 / 8;
      h3 {
        width: 66%;
      }
    }
    .illustration {
      grid-column: 7 / 13;
    }
  }

  #whoWeAre {
    padding: 8rem 0rem 2rem 0rem;
    height: 50vh;
    .pitch {
      grid-column: 7 / 13;
    }
    .illustration {
      grid-column: 1 / 8;
      // padding-bottom: 0;
    }
    .grid-interest {
      place-items: center start;
    }
  }

  #joinUs {
    padding: 8rem 0rem 2rem 0rem;
    place-items: center center;
    .pitch {
      grid-column: 1 / 6;
      h2 {
        margin: 0 0 1.5rem 0;
        width: 66%;
      }
    }
    .illustration {
      grid-column: 7 / 13;
      grid-row: 1;
    }
  }

  #social {
    place-items: center center;
    .pitch {
      grid-column: 7 / 13;
      padding: 0 0 0 4rem;
    }
    .illustration {
      grid-column: 1 / 7;
    }
  }
}
</style>