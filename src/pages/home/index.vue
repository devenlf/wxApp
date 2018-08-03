<template>
  <div class="container">
       <v-page1 :Id="0" v-if="false"></v-page1>
       <v-page2 :Id="1" v-if="false"></v-page2>
       <v-page3 :Id="2" v-if="false"></v-page3>
       <v-page4 :Id="3" v-if="false"></v-page4>
       <v-footer></v-footer>
  </div>
</template>

<script>
import footer from '@/components/footer'
import page1 from '@/pages/page1'
import page2 from '@/pages/page2'
import page3 from '@/pages/page3'
import page4 from '@/pages/page4'
export default {
  data() {
    return {
      current: "homepage"
    };
  },

  components: {
    'v-footer':footer,
    'v-page1':page1,
    'v-page2':page2,
    'v-page3':page3,
    'v-page4':page4
  },

  methods: {
    isShowPageId(){
      console.log(this.$store) 
    }
  },

  created() {
   this.isShowPageId()
  }
};
</script>

<style>
.container {
  width: 100%;
}
</style>
