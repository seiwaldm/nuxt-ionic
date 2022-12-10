<script setup lang="ts">
definePageMeta({ alias: ["/"] });
</script>

<template>
  <ion-page>
    <layout-app-header />
    <ion-content class="ion-padding">
      <h1>Home</h1>
      <ion-button>Default</ion-button>
      <ion-button fill="outline">Outline</ion-button>
      <ion-button color="success">Success</ion-button>
      <ion-button color="warning">Warning</ion-button>
      <ion-button color="danger">Danger</ion-button>
    </ion-content>
  </ion-page>
</template>
