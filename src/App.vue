<template>
  <div class="chat-container">
    <chat-component ref="chat"></chat-component>
    <list-component></list-component>
    
  </div>
</template>

<script>
import ChatComponent from './components/ChatComponent';
import ListComponent from './components/ListComponent';

export default {
  name: 'App',
  components:{
    'chat-component':ChatComponent,
    'list-component':ListComponent,
  },
  mounted(){
    this.$refs.chat.$el.style.height = `${window.innerHeight}px`;
  }
  
}

// export const a = 10;
// export const b = 20;
</script>

<style>
  .chat-container{
    width: 1000px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 3fr 1fr;

}
</style>