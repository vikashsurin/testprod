<script>
</script>

<section>
  <div id="tool-section">
    <div class="tool-category">
      <p>uiux</p>
      <div class="tool-list">
        <span id="figma">Figma</span>
        <span id="sketch">Sketch</span>
        <span id="figjam">Figjam</span>
        <span id="miro">Miro</span>
        <span id="xd">Xd</span>
      </div>
    </div>
    <div class="tool-category">
      <p>photo editing and vector graphics</p>
      <div class="tool-list">
        <span id="photoshop">Photoshop</span>
        <span id="illustrator">Illustrator</span>
      </div>
    </div>
    <div>
      <div class="tool-category">
        <p>art</p>
        <div class="tool-list">
          <span id="procreate">Procreate</span>
        </div>
      </div>
    </div>
  </div>
  <hr style="border-color: var(--title-color);" />
  <!-- ui ux process -->
  <div id="process">
    <h3>ux design process</h3>
    <div id="process-list">
      <p>
        <span>1.</span>
        <span>Empathize</span>
        <span />
      </p>
      <p>
        <span>2.</span>
        <span> Define </span>
      </p>
      <p>
        <span>3.</span>
        <span>Ideate</span>
      </p>
      <p>
        <span>4.</span>
        <span>Prototype</span>
      </p>
      <p>
        <span>5.</span>
        <span>Test</span>
      </p>
    </div>
  </div>

  <div>
    <img id="wireframe" src="/wireframe.JPG" alt="" />
  </div>
</section>

<style lang="scss">
  :root {
    --title-color: rgb(155, 155, 155);
  }
  section {
    margin: 0% 20%;
    #tool-section {
      display: grid;
      grid-template-columns: repeat(1, 1fr);
      align-items: center;
      gap: 100px;
      padding: 200px 0px;
      .tool-category {
        p {
          font-weight: 700;
          font-size: 2em;
          color: var(--title-color);
        }
        .tool-list {
          display: flex;
          flex-wrap: wrap;
          border-left: 5px solid var(--title-color);
          //   grid-template-columns: repeat(3, 1fr);
          span {
            font-family: Arial Black, Helvetica, sans-serif;
            font-size: 50px;
            opacity: 50%;
            transition: ease-in-out 200ms;
            transform: skew(-5deg, 0deg);
            padding: 0px 50px;
          }
          span:hover {
            opacity: 100%;
            background-color: black;
            transform: scale(1.3) skew(0deg, 0deg) translate(50px, 0px);
          }
        }
      }

      #figma {
        display: block;
        color: #794ac4;
      }
      #figjam {
        color: #ee7a69;
        font-weight: 100;
      }
      #miro {
        color: #f8d254;
      }
      #photoshop {
        color: #57a6f8;
      }
      #illustrator {
        color: #f09e38;
      }
      #sketch {
        color: #e1703b;
      }
      #xd {
        color: #ed6cef;
      }
      #procreate {
        color: #da80c7;
      }
    }

    // DESIGN PROCESS
    #process {
      #process-list {
        border-left: 5px solid limegreen;
        padding-left: 20px;
      }
      h3 {
        font-size: 5em;
        color: var(--title-color);
      }
      padding: 300px 0px;
      color: white;
    }
  }

  #wireframe {
    height: 400px;
  }
</style>
