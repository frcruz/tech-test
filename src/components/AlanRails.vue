<template>
  <div>
    <md-card>
      <md-card-media-cover md-solid>
        <md-card-media md-ratio="4:3">
          <img src="../assets/alan-rails.jpeg" alt="Alan Rails">
        </md-card-media>

        <md-card-area>
          <md-card-header>
            <span class="md-title">Alan Rails</span>
          </md-card-header>
        </md-card-area>
      </md-card-media-cover>
      <md-card-content>
        <md-list>
          <md-list-item>
            <span class="left">STATUS</span> 
            <span class="right">Dead</span>
          </md-list-item>
          <md-divider></md-divider>
          <md-list-item>
            <span class="left">SPECIES</span> 
            <span class="right">Human, Superhuman (Ghost trains summoner)</span>
          </md-list-item>
          <md-divider></md-divider>
          <md-list-item>
            <span class="left">GENDER</span> 
            <span class="right">Male</span>
          </md-list-item>
          <md-divider></md-divider>
          <md-list-item>
            <span class="left">ORIGIN</span> 
            <span class="right">unknown</span>
          </md-list-item>
          <md-divider></md-divider>
          <md-list-item>
            <span class="left">LAST LOCATION</span> 
            <span class="right">Worldender's lair</span>
          </md-list-item>
        </md-list>
      </md-card-content>
    </md-card>
  </div>
</template>

<script>
export default {
  name: 'AlanRails',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
span.left {
  float: left;
}
span.right {
  float: right;
}

.md-card {
  margin: 4px;
  display: inline-block;
  vertical-align: top;
}
.md-list-item span {
  white-space: normal;
}
</style>
