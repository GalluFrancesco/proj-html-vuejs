<template>
  <div id="app">
    <header-box :contentList="headerContent"/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox
  },
  data(){
    return{
      headerContent:[
        {
          id:'HC01',
          image:'course-9-f-img.jpg',
          title:'Contemporary Ideas',
          text:'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci officia voluptas consequuntur omnis! Numquam animi est necessitatibus accusantium cupiditate expedita voluptates tenetur, magnam ut, excepturi repudiandae, iusto eos qui provident?'
        },
        {
          id:'HC02',
          image:'course-5-f-img.jpg',
          title:'Titolo 2',
          text:'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci officia voluptas consequuntur omnis! Numquam animi est necessitatibus accusantium cupiditate expedita voluptates tenetur, magnam ut, excepturi repudiandae, iusto eos qui provident?'
        },
        {
          id:'HC03',
          image:'course-12-f-img.jpg',
          title:'Titolo 3',
          text:'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci officia voluptas consequuntur omnis! Numquam animi est necessitatibus accusantium cupiditate expedita voluptates tenetur, magnam ut, excepturi repudiandae, iusto eos qui provident?'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
  @import url('https://use.fontawesome.com/releases/v5.7.1/css/all.css');
  @import './style/main.scss';
</style>
