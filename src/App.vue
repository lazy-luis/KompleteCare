<script setup>
import SideBar from './components/SideBar.vue';
import MainBody from './components/MainBody.vue';
</script>

<template>
  <div class="mainContainer">
    <div class="sideContainer">
      <SideBar />
    </div>
    <div class="bodyContainer">
      <MainBody />
    </div>
  </div>
</template>

<style>
@import url('/main.css');
  .mainContainer{
    background: #F5F5FB;
    min-height: 100vh;
    min-width: 100%;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
  }
  .mainContainer .sideContainer {
    width: 18%;
    background: #FFFFFF;
    position: fixed;
    clear: both;
  }
  .mainContainer .bodyContainer {
    width: 82%;
    clear: both;
    margin-left: 18%;
  }
  @media (max-width: 600px) {
    .mainContainer .sideContainer {
      display: none;
    }
    .mainContainer .bodyContainer {
      width: 100%;
      margin-left: 0%;
    }
  }
</style>
