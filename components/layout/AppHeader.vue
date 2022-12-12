<script setup lang="ts">
import { Icon } from "@iconify/vue";
const router = useIonRouter();

const showMenu = ref(false);
</script>

<template>
  <ion-header>
    <ion-toolbar pr-4>
      <div flex gap-4>
        <ion-title router-link="/" cursor-pointer>Go Home</ion-title>

        <Icon icon="logos:nuxt" />
        <Icon icon="logos:ionic" />

        <Icon
          @click="showMenu = true"
          id="menuButton"
          icon="ion:menu"
          cursor-pointer
        />
        <ion-popover
          trigger="menuButton"
          @didDismiss="showMenu = false"
          :is-open="showMenu"
        >
          <ion-content class="ion-padding">
            <ion-button @click="router.push('/test')">test</ion-button>
          </ion-content>
        </ion-popover>
      </div>
    </ion-toolbar>
  </ion-header>
</template>
