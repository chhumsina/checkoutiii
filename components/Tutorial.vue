<template>
  <vue-bottom-sheet ref="myBottomSheet">
    <div style="text-align: center;">
      <h1>Lorem Ipsum</h1>
    <h2>What is Lorem Ipsum?</h2>
    <input/>
    <button @click="reloadme">Reload</button>
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
    setTimeout(() => {
      
    this.open()
      }, 500);
  },
  methods: {
    open() {
      this.$refs.myBottomSheet.open();
    },
    close() {
      this.$refs.myBottomSheet.close();
    },
    reloadme(){

      location.reload()
    }
  }
}
</script>
