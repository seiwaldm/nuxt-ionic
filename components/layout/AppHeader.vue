<script setup lang="ts">
import { Icon } from "@iconify/vue";
</script>

<template>
  <ion-header>
    <ion-toolbar pr-4>
      <div flex gap-4>
        <ion-title>Home</ion-title>

        <Icon icon="logos:nuxt" />
        <Icon icon="logos:ionic" />
        <Icon id="click-trigger" icon="ion:menu" cursor-pointer />
        <ion-popover trigger="click-trigger" trigger-action="click">
          <ion-content class="ion-padding">Hello World!</ion-content>
        </ion-popover>
      </div>
    </ion-toolbar>
  </ion-header>
</template>
