<template>
  <ion-page>
    <ion-tabs>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="intro" href="/intro">
          <ion-icon :icon="homeOutline" />
          <ion-label>Intro</ion-label>
        </ion-tab-button>
          
        <ion-tab-button tab="topics" href="/topics">
          <ion-icon :icon="albumsOutline" />
          <ion-label>Topics</ion-label>
        </ion-tab-button>
        
        <ion-tab-button tab="map" href="/map">
          <ion-icon :icon="mapOutline" />
          <ion-label>Map</ion-label>
        </ion-tab-button>
        
        <ion-tab-button tab="dates" href="/dates">
          <ion-icon :icon="calendarNumberOutline" />
          <ion-label>Dates</ion-label>
        </ion-tab-button>
        
        <ion-tab-button tab="tickets" href="/tickets">
          <ion-icon :icon="cartOutline" />
          <ion-label>Tickets</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script >
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage } from '@ionic/vue';
import { 
  homeOutline, 
  albumsOutline,
  mapOutline,
  calendarNumberOutline,
  cartOutline,
 } from 'ionicons/icons';

export default {
  name: 'PickUp',
  components: { IonLabel, IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage },
  setup() {
    return {
      homeOutline, 
      albumsOutline,
      mapOutline,
      calendarNumberOutline,
      cartOutline,
    }
  }
}
</script>
