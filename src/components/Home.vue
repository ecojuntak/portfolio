<template>
  <div>
    <div class="head">
      <profile/>
      <description/>
    </div>

    <div>
      <blog/>
    </div>

    <div>
      <foot/>
    </div>
  </div>
</template>

<script>
import Profile from "./Profile"
import Description from "./Description"
import Blog from "./Blog"
import Foot from "./Footer"

export default {
  name: "Home",
  data() {
    return {
      msg: "Hi! I'm Eko Simanjuntak, Passionate Software Engineer"
    };
  },
  components: {
    Profile,
    Description,
    Blog,
    Foot
  }
};
</script>

<style>
@import 'https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Material+Icons';
@import url("https://fonts.googleapis.com/css?family=K2D");

.head {
  background-color: rgba(33, 33, 33, 1);
  display: flow-root;
  padding-bottom: 100px;
}

@keyframes blink-animation {
  from {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@-webkit-keyframes blink-animation {
  from {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
