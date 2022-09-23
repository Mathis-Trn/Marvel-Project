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

<script>
import HerosItem from './HerosItems.vue'
import ThorIcon from './icons/IconThor.vue'
import SpiderManIcon from './icons/IconSpiderMan.vue'
import HawkeyeIcon from './icons/IconHawkeye.vue'
import IronManIcon from './icons/IconIronMan.vue'
import CptAmericaIcon from './icons/IconCptAmerica.vue'
import BlackWidowIcon from './icons/IconBlackWidow.vue'
import HulkIcon from './icons/IconHulk.vue'
import OpenCloseProfile from './openCloseProfile.vue'

export default {
  data() {
    return {
      // CREER TOI UN TABLEAU D'OBJECT ICI AVEC DES INFOS SUR TES HEROS ET DANS TON TEMPLATE REGARDE COMMENT MARCHE LES V-FOR ET DANS TA
      // FONCTION functionToOpenCloseProfile TU LUI ENVOIS LES DONNEES DU HERO
      heros: [
        {
          name: "Thor",
          power: "Thunder"
        }
      ]
    }
  },
  methods: {
    functionToOpenCloseProfile(val) {
      console.log(val)
    }
  },
  components: {
    HerosItem,
    ThorIcon,
    SpiderManIcon,
    HawkeyeIcon,
    IronManIcon,
    CptAmericaIcon,
    BlackWidowIcon,
    HulkIcon,
    OpenCloseProfile,
  }
}
</script>

<template>
  <HerosItem>
    <template #icon >
      <button @click="functionToOpenCloseProfile(this)"> <ThorIcon /> </button>
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

