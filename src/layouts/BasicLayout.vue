<template>
  <div id="basicLayout">
    <GloballHeader />
    <a-layout>
      <a-layout-header class="header"></a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer">
        <a href="https://github.com/" target="_blank">By氯化镁 </a>
      </a-layout-footer>
    </a-layout>
  </div>
</template>

<script setup lang="ts">
import GloballHeader from "@/components/GloballHeader.vue";
</script>

<style scoped>
#basicLayout .footer {
  baground-color: #efefef;
  text-align: center;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
}

#basicLayout .content {
  padding: 20px;
  background: linear-gradient(to right, #efefef, #fff);
}

#basicLayout .header {
  background: #efefef;
  height: auto;
  padding: 5px;
}
</style>
