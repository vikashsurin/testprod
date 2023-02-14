<script>
  let src = "/profile.jpg";
</script>

<section>
  <div id="intro">
    <p1>hi, my name is</p1>
    <p2>Vikash surin</p2>
    <p3>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos,
      excepturi! Rerum quas placeat eos ducimus earum? Inventore voluptatem
      saepe amet incidunt debitis odio, repellendus enim consequuntur dolores
      ipsam assumenda nesciunt!
    </p3>
  </div>
  <div class="profile-pic">
    <img {src} alt="" />
    <div id="move" />
  </div>
  <div />
  <div id="resume">
    <button> Resume </button>
  </div>
  <div class="images-cont">
    <div class="img-cont">
      <h2>Ui Design</h2>
      <img class="image" src="/ss.png" alt="" />
      <img class="image" src="/ss2.png" alt="" />
      <img class="image" src="/ss3.png" alt="" />
      <!-- <a class="more" href="##">see more >></a> -->
    </div>

    <div class="img-cont">
      <h2>Photography</h2>
      <img class="image" src="/DSC05412.jpg" alt="" />
      <img class="image" src="/DSC05770.jpg" alt="" />
      <img class="image" src="/DSC04226.jpg" alt="" />
      <img class="image" src="/DSC05757.jpg" alt="" />
      <!-- <a href="##"> sdfs </a> -->
    </div>

    <div class="img-cont">
      <h2>Digital Paintings</h2>
      <img class="image" src="/boat.JPG" alt="" />
      <img class="image" src="/boy.JPG" alt="" />
      <img class="image" src="/arch.JPG" alt="" />
      <img class="image" src="/drink.JPG" alt="" />
      <img class="image" src="/eye.JPG" alt="" />
      <!-- <a href="##"> see more >> </a> -->
    </div>
  </div>
  <!-- EXPERIMENTS -->
  <a href="" id="ec">Experiments - Curiosity</a>
</section>

<!-- styles -->
<style lang="scss">
  section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 100px 0px;
    margin: 1% 20%;
    color: white;
    padding: 200px 0px;
    #intro {
      p1 {
        display: block;
        padding: 20px 0px;
      }
      p2 {
        display: block;
        font-size: 4em;
        font-weight: 700;
        padding: 20px 0px;
      }
      p3 {
        display: block;
        font-weight: 500;
      }
    }
  }
  .profile-pic {
    width: 100%;
    height: 300px;
    position: relative;
    img {
      z-index: 999;
    }
    #move {
      z-index: -1;
      background-color: black;
      height: inherit;
      width: 100%;
      position: absolute;
      top: 0;
      left: 0;
      transition: transform ease-in-out 200ms;
    }
    img {
      height: inherit;
      width: auto;
      transition: transform ease-in-out 200ms;
    }
  }
  .profile-pic:hover img {
    transform: translate(10px, -10px);
  }

  .profile-pic:hover div {
    transform: translate(-10px, 10px);
  }

  #resume {
    button {
      background-color: teal;
      border: none;
      border-radius: 2px;
      padding: 10px 25px;
      font-weight: 300;
      color: white;
      transition: background-color ease-in-out 200ms;
    }
    button:hover {
      background-color: rgb(0, 102, 175);
    }
  }
  .images-cont {
    grid-column: 1 / span 2;
    .img-cont {
      padding: 100px 0px;

      a {
        display: flex;
      }
    }
  }

  .image {
    height: 200px;
    opacity: 0.8;
    transition: transform ease-in-out 300ms;
  }
  .image:hover {
    opacity: 1;
    box-shadow: 0px 0px 30px rgb(30, 30, 30);
    transform: translate(0px, 10px);
  }

  // experiment
  #ec {
    color: var(--title-color);
    grid-column: 1 / span 2;
    justify-self: center;
  }
</style>
