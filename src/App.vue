<template>
  <div class="container">
    <Human /><!--3. 普通のHTMLタグのようにHumanコンポーネントを書く-->
    <Human />
    <Human />
    <Human />
    <Human />
    <Human />
    <Human />
  </div>
</template>


<script>
import Human from "@/components/Human.vue"; //1. HumanコンポーネントをHuman.vueから読み込む

// @はsrcディレクトリを指すよ！（絶対パス）
export default {
  components: {
    Human, //2. HumanコンポーネントをApp.vueのなかで使えるように登録する
  },
};
</script>

<style scoped>
.container {
  display: flex;
}
</style>
