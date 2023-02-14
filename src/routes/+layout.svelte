<nav>
  <logo><span id="vikash"> vikashsurin.</span><span id="com">com</span></logo>
  <links>
    <a href="/">about</a>
    <a href="/work">case studies</a>
    <a href="/tools">tools</a>
    <a href="/blog">blog</a>
    <!-- <a href="#">theme</a> -->
  </links>
</nav>

<slot />

<footer>
  <div id="copyright"><span>© 2021-2022 designed by vikash surin</span></div>
  <div id="portfolio-section">
    <div id="portfolio-list">
      <a href="##" class="list-item" id="behance">behance</a>
      <a href="##" class="list-item" id="dribble">dribble</a>
      <a href="##" class="list-item" id="artstation">artstation</a>
      <a href="##" class="list-item" id="shutterstock">shutterstock</a>
    </div>
  </div>

  <div id="social-section">
    <div id="social-list">
      <a href="##" class="social-item list-item" id="facebook">facebook</a>
      <a href="##" class="social-item list-item" id="twitter">twitter</a>
      <a href="##" class="social-item list-item" id="linkedin">linkedIn</a>
      <a href="##" class="social-item list-item" id="instagram">instagram</a>
    </div>
  </div>
</footer>

<style lang="scss">
  nav {
    position: sticky;
    z-index: 10;
    top: 0px;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    padding: 1% 3%;
    background-color: #1e2025;
    border-bottom: 1px solid #484c56;
    align-items: center;

    logo {
      font-size: 1.5em;
      font-weight: 600;

      #vikash {
        color: #bdbdbd;
      }
      #com {
        color: #58a0cc;
      }
    }
  }

  links {
    grid-column: 4/5;
    justify-self: flex-end;

    a {
      text-decoration: none;
      color: whitesmoke;
      transition: ease-in-out 200ms;
      padding: 0em 1em;
    }
    a:hover {
      color: #e4a345;
      font-weight: 500;
    }
  }

  // footer
  footer {
    height: 10%;
    padding: 3% 3%;
    position: relative;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    color: white;
    background-color: #2b2e37;
    align-items: flex-end;

    #copyright {
      color: #bdbdbd;
    }
    #portfolio-section {
      a {
        text-decoration: none;
        color: whitesmoke;
        font-weight: 700;
        font-size: 1em;
        padding: 0px 10px;
        opacity: 50%;
        transition: all ease-in-out 200ms;
      }
      a:hover {
        opacity: 100%;
      }
      #behance {
        color: #1769ff;
      }
      #dribble {
        color: #ea4c89;
      }
      #shutterstock {
        color: #de3f2a;
      }
      #artstation {
        color: #51acea;
      }
    }

    #social-section {
      #social-list {
        a {
          text-decoration: none;
          color: whitesmoke;
          font-weight: 700;
          font-size: 1em;
          padding: 0px 10px;
          opacity: 50%;
          transition: opacity ease-in-out 200ms;
        }
        a:hover {
          opacity: 100%;
        }

        #facebook {
          color: #58a0cc;
        }
        #twitter {
          color: #1da1f2;
        }
        #linkedin {
          color: #0077b5;
        }
        #instagram {
          color: #c13584;
        }
      }
    }
  }
</style>
