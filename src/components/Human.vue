<template>
  <div class="Human">
    <div class="atama">
      <div v-if="isLaughing">🤣</div>
      <div v-else>😊</div>
    </div>
    <div class="karada" v-on:click="makeLaugh">
      <div>💪</div>
      <div><slot /></div>
      <div>💪</div>
    </div>

    <div class="ashi">
      <div>🦵🦵</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    clothes: { type: String, default: "👚" },
  },

  methods: {
    makeLaugh() {
      this.isLaughing = true;
    },
  },
};
</script>

<style>
.Human {
  width: 10rem;
  font-size: 3rem;
  text-align: center;
}
.karada {
  display: flex;
}
.container {
  display: flex;
  font-size: 4rem;
}
</style>
