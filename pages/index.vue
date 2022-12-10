<script setup lang="ts">
import { menu } from "ionicons/icons";
import { Icon } from "@iconify/vue";
definePageMeta({ alias: ["/"] });
</script>

<template>
  <ion-page>
    <ion-header>
      <ion-toolbar pr-4>
        <ion-title>Home</ion-title>
        <div slot="end" flex gap-2>
          <ion-icon :icon="menu" />
          <Icon icon="ion:logo-ionic" />
          <Icon icon="logos:ionic" />
        </div>
      </ion-toolbar>
    </ion-header>
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
