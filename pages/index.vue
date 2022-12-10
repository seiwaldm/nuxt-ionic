<script setup lang="ts">
import { menu } from "ionicons/icons";
import { Icon } from "@iconify/vue";
definePageMeta({ alias: ["/"] });
</script>

<template>
  <ion-page>
    <ion-header>
      <ion-toolbar pr-4>
        <div flex gap-4>
          <ion-title>Home</ion-title>
          <ion-text>different Icons:</ion-text>

          <Icon icon="ion:logo-ionic" />
          <Icon icon="logos:ionic" />
          <Icon icon="ion:menu" />
          <ion-icon id="click-trigger" :icon="menu" />
          <ion-popover trigger="click-trigger" trigger-action="click">
            <ion-content class="ion-padding">Hello World!</ion-content>
          </ion-popover>
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
