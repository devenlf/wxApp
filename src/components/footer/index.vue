<template>
  <div class="footer">
   <i-tab-bar color="#f759ab" bindchange="handleChange">
    <i-tab-bar-item :Id="0" @click="getId($event)" class="card" key="homepage" icon="homepage" current-icon="homepage_fill" title="首页"></i-tab-bar-item>
    <i-tab-bar-item :Id="1" @click="getId($event)"  class="card" key="group" icon="group" current-icon="group_fill" title="朋友"></i-tab-bar-item>
    <i-tab-bar-item :Id="2" @click="getId($event)"  class="card" key="remind" icon="remind" current-icon="remind_fill" title="通知"></i-tab-bar-item>
    <i-tab-bar-item :Id="3" @click="getId($event)"  class="card" key="mine" icon="mine" current-icon="mine_fill" title="我的"></i-tab-bar-item>
</i-tab-bar>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },

  components: {},

  methods: {
    getId(e){
      console.log(e.currentTarget.dataset.eventid)
    }
  },

  created() {}
};
</script>

<style>
.footer {
  width: 100%;
  height: 8%;
  position: fixed;
  bottom: 0px;
  background: #ffffff
}
.card{
  float: left;
  width: 25%;
  
}
</style>
