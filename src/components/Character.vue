<template>
    <md-card>
      <md-card-media-cover md-solid>
        <md-card-media md-ratio="4:3">
          <img v-bind:src="img" v-bind:alt="name">
        </md-card-media>

        <md-card-area>
          <md-card-header>
            <span class="md-title">{{name}}</span>
          </md-card-header>
        </md-card-area>
      </md-card-media-cover>
      <md-card-content>
        <md-list>
          <md-list-item v-for="(trait, index) in traits" :key="index">
            <span class="left">{{trait}}</span> 
            <span class="right" v-if="trait == 'STATUS'">{{status}}</span>
            <span class="right" v-if="trait == 'SPECIES'">{{species}}</span>
            <span class="right" v-if="trait == 'GENDER'">{{gender}}</span>
            <span class="right" v-if="trait == 'ORIGIN'">{{species}}</span>
            <span class="right" v-if="trait == 'LAST LOCATION'">{{location}}</span>
          </md-list-item>
        </md-list>
      </md-card-content>
    </md-card>
</template>

<script>
export default {
  name: 'Character',
  data() {
      return {
          traits: ['STATUS', 'SPECIES', 'GENDER', 'ORIGIN', 'LAST LOCATION'],
          name: "",
          status: "",
          species: "",
          gender: "",
          origin: "",
          location: "",
          img: ""
      }
  },
 // traits = ['STATUS', 'SPECIES', 'GENDER', 'ORIGIN', 'LAST LOCATION'];
  async mounted() {
      var num1 = Math.floor(Math.random() * 671);
      var url = 'https://rickandmortyapi.com/api/character/' + num1
      let response = await fetch(url);   
      if(response.ok) {
          let json = await response.json();
          console.log(json);
          this.name = json['name'];
          this.status = json['status'];
          this.species = json['species']
          this.gender = json['gender'];
          this.origin = json['origin']['name'];
          this.location = json['location']['name'];
          this.img = json['image']
      }
  }
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
  width: 320px;
  height: 540px;
  margin: 4px;
  display: inline-block;
  vertical-align: top;
}
.md-list-item span {
  white-space: normal;
}
</style>
