<template>
    <page-layout>
        <div class="home">
          <container>
            <h1>A simple cron-like job scheduler for Node.js</h1>
            <div class="demo-container">
              <demo></demo>
            </div>
            <router-link to="/docs" class="btn btn-primary btn-large">Getting Started</router-link>
          </container>
        </div>
    </page-layout>
</template>

<script>
import PageLayout from '../layouts/page-layout.vue';
import Container from '../components/container.vue';
import Demo from '../components/demo.vue';

export default {
  components: {
    PageLayout,
    Container,
    Demo
  }
}
</script>

<style lang="scss">
  .home {
    text-align: center;
    height: 100%;
    margin-top: 100px;

    button {
      margin-top: 30px;
    }
  }

  .demo-container {
    width: 70%;
    @media screen and (max-width: 850px){
      width: 95%;
    }
    margin-left: auto;
    margin-right: auto;
    margin-top: 40px;
  }
</style>

