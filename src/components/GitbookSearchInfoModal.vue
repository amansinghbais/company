<template>
  <ion-list>
    <ion-content>
      <ion-list>
        <ion-list-header>{{ queryString  }}</ion-list-header>

        <ion-item lines="none">
          <ion-label>
            {{ answer.text }}
          </ion-label>
        </ion-item>
      </ion-list>
    </ion-content>
  </ion-list>
</template>
<script setup lang="ts">
import { IonContent, IonItem, IonLabel, IonList, IonListHeader } from "@ionic/vue";
import { defineProps } from "vue";

const props = defineProps(["queryString", "answer"]);
</script>
