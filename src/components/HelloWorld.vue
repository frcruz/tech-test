<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <article>
    <div>
      <img src="images/alan-rails.jpeg" alt="Alan Rails">
        <h5>Alan Rails</h5>
    </div>
    <div>
      <div>
        <div>STATUS</div>
        <div>Dead</div>
      </div>
      <div>
        <div>SPECIES</div>
        <div>Human, Superhuman (Ghost trains summoner)</div>
      </div>
      <div>
        <div>GENDER</div>
        <div>Male</div>
      </div>
      <div>
        <div>ORIGIN</div>
        <div>unknown</div>
      </div>
      <div>
        <div>LAST LOCATION</div>
        <div>Worldender's lair</div>
      </div>
    </div>
  </article>
  <md-card>
      <md-card-media-cover md-solid>
        <md-card-media md-ratio="4:3">
          <img src="/../assets/alan-rails.jpeg" alt="Alan Rails">
        </md-card-media>

        <md-card-area>
          <md-card-header>
            <span class="md-title">Solid background</span>
            <span class="md-subhead">4/3 image</span>
          </md-card-header>
        </md-card-area>
      </md-card-media-cover>
    </md-card>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
