<template>
  <div id="app">
    <Header :Name='Name' />
    <div class='content'>
      <ImageBox />
      <socials :SocialMedia='SocialMedia' />
    </div>
    <NavBar />
 
  </div>
</template>

<script>
import axios from 'axios';
import socials from '@/components/Socials.vue';
import ImageBox from '@/components/ImageBox.vue';
import Header from '@/components/Header.vue';
import NavBar from '@/components/NavBar.vue';

window.axios = axios;

// const url = 'https://hirng-x2021.glitch.me/api';

export default{
  name: 'app',
  components: {
    socials,
    ImageBox,
    Header,
    NavBar
  },
  data(){
    return{
    SocialMedia: {
      twitter: "aquilaveion",
      instagram: "aquilaveionofficial",
      snapchat: "aquilaveionsnaps",
      email: "aquilaveion@aquil.com"
     },
     Name: "AQUILA AVEION",
    }
  },
  // mounted(){
  //   axios.get(url).then(res => {
  //     this.SocialMedia = res.data.social_media;
  //     this.Name = res.data.name;
  //   },[])
  // }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rajdhani:wght@300&display=swap');

html, body {
  font-family: 'Rajdhani', sans-serif;
  margin: 0px !important;
  padding: 0px !important;
  background: linear-gradient(90deg, #bd0f4d 50%, #cb2964 50%);
  color: #f4d8e2;
}

#app {
  font-family: 'Rajdhani', sans-serif;
  text-align: center;
}

.content{
  display: flex;

}
</style>
