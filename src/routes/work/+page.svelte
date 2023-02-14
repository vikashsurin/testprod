<section>
  <div class="case">
    <a href="/work/details/gobook">GoBook</a>
    <span>This app is a basic app</span>
  </div>
  <div class="case">
    <h2>goBook</h2>
    <span>This app is a basic app</span>
  </div>
  <div class="case">
    <h2>goBook</h2>
    <span>This app is a basic app</span>
  </div>
  <div class="case">
    <h2>goBook</h2>
    <span>This app is a basic app</span>
  </div>
</section>

<style lang="scss">
  section {
    min-height: 100vh;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    margin: 100px 300px;
    color: whitesmoke;
    .case {
      background-color: grey;
      height: 200px;
      width: 200px;
      display: grid;
      align-content: center;
      justify-content: center;
      padding: 30px;
    }
  }
</style>
