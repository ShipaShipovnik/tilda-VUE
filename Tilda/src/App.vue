<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HeadBar from './components/HeadBar.vue'
import Footer from './components/Footer.vue'

</script>

<template>
  <HeadBar />
  <div class="content-wrapper">
    <router-view v-slot="{ Component }">
      <transition name="fade">
        <component :is="Component" />
      </transition>
    </router-view>
  </div>
  <Footer />
</template>

<style>
.fade-enter-active,
.fade-leave-active {
  transition-property: opacity;
  transition-duration: .25s;
}

.fade-enter-active {
  transition-delay: .25s;
}

.fade-enter,
.fade-leave-active {
  opacity: 0;
}
</style>