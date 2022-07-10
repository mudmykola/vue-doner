<template>
<v-navigation-drawer app color="white" right width="300">
  <v-list class=" mt-1" subheader two-line >
    <v-list-item>
 <v-list-item-avatar rounded >
      <v-img src="image-1.png"></v-img>
    </v-list-item-avatar>
    <v-list-item-content>
      <v-list-item-subtitle>Адміністратор</v-list-item-subtitle>
      <v-list-item-title>Микола Мудь</v-list-item-title>
    </v-list-item-content>
    <v-list-item-action >
      <v-badge bordered overlap color="red" dot>
        <v-icon >far fa-bell</v-icon>
      </v-badge>
    </v-list-item-action>
    </v-list-item>
   
  </v-list>
  <strong class=" ml-3">Додано в чек</strong>
  <v-list class=" mt-1" two-line subheader >
<v-list-item>
  <v-list-item-avatar rounded  color=" grey lighten-4" >
    <v-img src="doner-1.jpg"></v-img>
  </v-list-item-avatar>
  <v-list-item-content >
    <v-list-item-title class="subtitle-2">Донер XXL зі свинини гострий</v-list-item-title>
    <v-list-item-subtitle>X1 <v-btn plain color="#FF5722" dark small>Примітки
      <v-icon right>mdi-pencil</v-icon>
    </v-btn> </v-list-item-subtitle>
  </v-list-item-content>
  <v-list-item-action class=" caption"> &#8372;155</v-list-item-action>
</v-list-item>
  </v-list>
    <v-list class=" mt-1" two-line subheader >
<v-list-item>
  <v-list-item-avatar rounded  color=" grey lighten-4" >
    <v-img src="doner-2.jpg"></v-img>
  </v-list-item-avatar>
  <v-list-item-content >
    <v-list-item-title class="subtitle-2">Донер зі свининою</v-list-item-title>
    <v-list-item-subtitle>X1 <v-btn plain color="#FF5722" dark small>Примітки
      <v-icon right>mdi-pencil</v-icon>
    </v-btn> </v-list-item-subtitle>
  </v-list-item-content>
  <v-list-item-action class=" caption"> &#8372;102</v-list-item-action>
</v-list-item>
  </v-list>
    <v-list class=" mt-1" two-line subheader >
<v-list-item>
  <v-list-item-avatar rounded  color=" grey lighten-4" >
    <v-img src="doner-3.jpg"></v-img>
  </v-list-item-avatar>
  <v-list-item-content >
    <v-list-item-title class="subtitle-2">Донер з куркою</v-list-item-title>
    <v-list-item-subtitle>X1 <v-btn plain color="#FF5722" dark small>Примітки
      <v-icon right>mdi-pencil</v-icon>
    </v-btn> </v-list-item-subtitle>
  </v-list-item-content>
  <v-list-item-action class=" caption"> &#8372;165</v-list-item-action>
</v-list-item>
  </v-list>
  <v-toolbar flat color="rgba(0,0,0,0)">
    <strong>Підсумок</strong><v-spacer></v-spacer><strong>&#8372;422</strong>
  </v-toolbar>
  <v-toolbar class="mt-n6" color="rgba(0,0,0,0)" flat>
    <span >ПДВ(20%)</span><v-spacer></v-spacer><span>&#8372;84.40</span>
  </v-toolbar>
  <v-divider class=" mx-4"></v-divider>
  <v-toolbar color="rgba(0,0,0,0)" flat>
  <span>Загальна сума</span><v-spacer></v-spacer><span>&#8372;506.40</span>
</v-toolbar>
<strong class=" ml-5">Спосіб оплати</strong>
<v-item-group class=" mt-n1" mandatory  >
  <v-container>
    <v-row justify=" center">
      <v-col cols="12" md="4">
       <v-item v-slot="{active, toggle}">
        <v-card :class="active ? 'borderme' : ''" class=" d-flex align-center rounded-lg" color="#f9fefe" dark height="70" @click="toggle" flat>
        <v-row>
          <v-col cols="12" md="12">
            <v-list-item class=" text-center mt-1" three-line>
              <v-list-item-content>
                <div>
                  <v-icon :color="active ? '#FF5722' : 'black'">fas fa-money-bill-wave</v-icon>
                </div>
                <v-list-item-subtitle class=" mt-n2 caption" :class="active ? 'brown--text' : 'black--text'">Готівкою</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        </v-card>
       </v-item>
      </v-col>

      <v-col cols="12" md="4">
       <v-item v-slot="{active, toggle}">
        <v-card :class="active ? 'borderme' : ''" class=" d-flex align-center rounded-lg" color="#f9fefe" dark height="70" @click="toggle" flat>
        <v-row>
          <v-col cols="12" md="12">
            <v-list-item class=" text-center mt-1" three-line>
              <v-list-item-content>
                <div>
                  <v-icon :color="active ? '#FF5722' : 'black'">fas fa-credit-card</v-icon>
                </div>
                <v-list-item-subtitle class=" mt-n2 caption" :class="active ? 'brown--text' : 'black--text'">Картою</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        </v-card>
       </v-item>
      </v-col>

      <v-col cols="12" md="4">
       <v-item v-slot="{active, toggle}">
        <v-card :class="active ? 'borderme' : ''" class=" d-flex align-center rounded-lg" color="#f9fefe" dark height="70" @click="toggle" flat>
        <v-row>
          <v-col cols="12" md="12">
            <v-list-item class=" text-center mt-1" three-line>
              <v-list-item-content>
                <div>
                  <v-icon :color="active ? '#FF5722' : 'black'">fas fa-qrcode</v-icon>
                </div>
                <v-list-item-subtitle class=" mt-n2 caption" :class="active ? 'brown--text' : 'black--text'">Додатком</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        </v-card>
       </v-item>
      </v-col>
    </v-row>
  </v-container>
</v-item-group>
</v-navigation-drawer>

</template>

<script>
export default {

}
</script>

<style>
.v-card.borderme{
  border: 2px solid #FF5722;
}
.col-12{
  padding: 5px;
}
.v-btn.widthoutupercase{
  text-transform: none;
}
</style>