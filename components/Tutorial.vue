<template>
  <vue-bottom-sheet ref="myBottomSheet">
    <div style="text-align: center;">
      <h1>Lorem Ipsum</h1>
    <h2>What is Lorem Ipsum?</h2>
    <input/>
    <p>
      <strong>Lorem Ipsum</strong> is simply dummy text
    </p>
    <p>
      <strong>Lorem Ipsum</strong> is simply dummy text
    </p>
    <p>
      <strong>Lorem Ipsum</strong> is simply dummy text
    </p>
    <p>
      <strong>Lorem Ipsum</strong> is simply dummy text
    </p>
    <p>
      <strong>Lorem Ipsum</strong> is simply dummy text
    </p>
    <p>
      <strong>Lorem Ipsum</strong> is simply dummy text
    </p>
    <button>Save</button>
    </div>
  </vue-bottom-sheet>
</template>

<script>
import  VueBottomSheet from "@webzlodimir/vue-bottom-sheet";

export default {
  components: {
    VueBottomSheet
  },
  mounted(){
    this.open()
  },
  methods: {
    open() {
      this.$refs.myBottomSheet.open();
    },
    close() {
      this.$refs.myBottomSheet.close();
    }
  }
}
</script>
