<template>
  <ion-page>
    <ion-tabs>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="Mapa" href="/tabs/tab1">
          <ion-icon :icon="map" />
          <ion-label>Mapa</ion-label>
        </ion-tab-button>
          
        <ion-tab-button tab="Reporte" href="/tabs/tab2">
          <ion-icon :icon="send" />
          <ion-label>Reporte</ion-label>
        </ion-tab-button>
        
        <ion-tab-button tab="Cerrar Sesion" href="/home">
          <ion-icon :icon="logOut" />
          <ion-label>Inicio</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script lang="ts">
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage } from '@ionic/vue';
import {map, send, logOut } from 'ionicons/icons';
// import MapaKaiser from "@/components/MapaKaiser.vue"

export default {
  name: 'Tabs',
  components: { IonLabel, IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage },
  setup() {
    return {
      map, 
      send, 
      logOut,
    }
  }
}
</script>