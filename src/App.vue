<template>
  <div id="app">
    <socials :SocialMedia='SocialMedia' />
    <ImageBox />
  </div>
</template>

<script>
import axios from 'axios';
import socials from '@/components/Socials.vue';
import ImageBox from '@/components/ImageBox.vue';

window.axios = axios;

const url = 'https://hirng-x2021.glitch.me/api';

export default{
  name: 'app',
  components: {
    socials,
    ImageBox,
  },
  data(){
    return{
     SocialMedia: [],
     Name: [],
    }
  },
  mounted(){
    axios.get(url).then(res => {
      this.SocialMedia = res.data.social_media;
      this.Name = res.data.name;
    },[])
  }
};
</script>

<style>
html, body {
  margin: 0px !important;
  padding: 0px !important;
  background: linear-gradient(90deg, #bd0f4d 60%, #cb2964 40%);
  color: #f4d8e2
}


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* height: 100%; */
}
</style>
