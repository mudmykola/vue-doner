<template>
<v-app :style="{ background: $vuetify.theme.themes.dark.background }">
 <the-side-bar/>
 <the-side-bar-right/>
</v-app>
 
</template>

<script>

import TheSideBar from '@/components/TheSideBar.vue'
import TheSideBarRight from '@/components/TheSideBarRight.vue'

  export default {
    name: 'TheHomeD',

    components: {
    TheSideBar,
    TheSideBarRight
},
  }
</script>
