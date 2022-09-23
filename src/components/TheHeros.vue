<style>
  .visible {
    height: 0;
    visibility: hidden;
    }
  .hidden {
    height: auto;
    visibility: visible;
    }
</style>

<script setup>
import HerosItem from './HerosItems.vue'
import ThorIcon from './icons/IconThor.vue'
import SpiderManIcon from './icons/IconSpiderMan.vue'
import HawkeyeIcon from './icons/IconHawkeye.vue'
import IronManIcon from './icons/IconIronMan.vue'
import CptAmericaIcon from './icons/IconCptAmerica.vue'
import BlackWidowIcon from './icons/IconBlackWidow.vue'
import HulkIcon from './icons/IconHulk.vue'
import OpenCloseProfile from './openCloseProfile.vue'
</script>

<template>
  <HerosItem>
    <template #icon >
      <button onclick="openCloseProfile(this);"> <ThorIcon /> </button>
    </template>
    <template #heading> Thor </template>
  <OpenCloseProfile>
    <template class="profile">
      <h3 class="profileContent hidden">
        Test 
      </h3>
    </template>
    </OpenCloseProfile>
  </HerosItem>
  

  <HerosItem>
    <template #icon>
      <button><SpiderManIcon /></button>
    </template>
    <template #heading> Spider-Man</template>

  </HerosItem>

  <HerosItem>
    <template #icon>
      <button><HawkeyeIcon /></button>
    </template>
    <template #heading> Hawkeye </template>
  </HerosItem>

  <HerosItem>
    <template #icon>
      <button><IronManIcon /></button>
    </template>
    <template #heading> Iron Man</template>

  </HerosItem>

  <HerosItem>
    <template #icon>
      <button><CptAmericaIcon /></button>
    </template>
    <template #heading> Captain America</template>

  </HerosItem>

  <HerosItem>
    <template #icon>
      <button><BlackWidowIcon /></button>
    </template>
    <template #heading> Black Widow</template>
  </HerosItem>

  <HerosItem>
    <template #icon>
      <button><HulkIcon /></button>
    </template>
    <template #heading> Hulk</template>
  </HerosItem>
</template>

