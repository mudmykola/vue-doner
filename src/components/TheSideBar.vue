<template>
<v-navigation-drawer v-model="drawer" app color="white" mini-variant mini-variant-width="100">
<v-avatar class=" d-block text--center mx-auto mt-4" size="40">
  <v-icon color="#FF5722"> fas fa-pepper-hot</v-icon>
</v-avatar>
<v-list class=" mt-4" flat>
 <v-list-item-group v-model="selectItem">
 <v-list-item v-for="(item,i) in items" :key="i" active-class="border" :ripple="false">
 <v-list-item-content>
  <v-icon v-text="item.icon"></v-icon>
  <v-list-item-subtitle class=" mt-3 caption" align="center" v-text="item.text" ></v-list-item-subtitle>
 </v-list-item-content>
 </v-list-item>
 </v-list-item-group>
</v-list>
<div style=" position:absolute; bottom: 20px; margin-left:auto; margin-right:auto; left:0; right:0; text-align:center; ">
<v-icon >fas fa-sign-out-alt</v-icon><br>
<span class=" caption">Вийти</span>
</div>
</v-navigation-drawer>
</template>

<script>
export default {
data: () => ({
  selectItem: 0,
  drawer: null,
  items: [
    {
      icon: 'fas fa-home', text:'Головна'
    },
     {
      icon: 'fas fa-hamburger', text:'Меню'
    },
     {
      icon: 'fas fa-history', text:'Історія'
    },
   
     {
      icon: 'fas fa-wallet', text:'Гаманець'
    },
     {
      icon: 'fas fa-percent', text:'Акції'
    },
     {
      icon: 'fas fa-cog', text:'Налаштування'
    },
  ],
})
}
</script>

<style>
.border{
  margin: 0 8px;
  background: #FF5722;
  border-radius: 20px;
  text-decoration: none;
}
.v-list-item-group .v-list-item--active {
  color: white;
}
.theme--light.v-list-item--active.v-list-item__subtitle, .theme--light.v-list-item.v-list-item__action-text{
    color: #fff;
}
</style>