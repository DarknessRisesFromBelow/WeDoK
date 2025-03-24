<script setup lang="ts">
import { ref, toRefs } from 'vue'
import Card from './Card.vue'


const props = defineProps<{
  BoardName: string
}>()


const name = ref(props.BoardName)
</script>

<template>
  <div class="BoardContainer">
    <input v-model="name" class="BoardName"></input>
    <Card/>
    <br/>
    <button class="addCardButton">+ Add a card</button>

  </div>
</template>

<style scoped>


  .BoardContainer
  {
    width: 272px;
    border-radius: 0.7em;
    box-shadow: 0px 0px 5px 1px black;
    padding-left: 1lvw; 
    padding-right: 1lvw;
    background: rgb(60,60,60); margin-right: 2lvh;
    padding-top: 2vh;
  }

  .BoardName
  {
    background: transparent;
    border: none;
    color: white;
    font-size: 1.5em;
    margin-bottom: 2vh;
    width: 262px;
  }

  .addCardButton{
    position: relative;
    height: 4vh;
    width: 90%;
    left: 5%;
    margin-bottom: 1vh;
    background: lightblue;
    border:none;
    border-radius: 0.5em;
    box-shadow: 0 0 3px 0.1px white;
  }
</style>