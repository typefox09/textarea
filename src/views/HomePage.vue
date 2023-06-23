<template>
  <ion-page>
    <ion-content>
        <button @click="isOpen = true">Open modal</button>
        <TestModal :isOpen="isOpen"/>
    </ion-content>
  </ion-page>
</template>

<script>
import { IonContent, IonPage } from '@ionic/vue';
import TestModal from "../components/TestModal.vue"

export default {
  name: "HomePage",
  components: {
    IonContent,
    IonPage,
    TestModal
  },
  data() {
    return {
      isOpen: false
    }
  }
}

</script>

<style scoped>
#container {
  width: 80%;
  margin-left: auto;
  margin-right: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  /* align-items: center; */
  height: 100%;
}

h1 {
  text-align: center;
}
.continer2 {
  flex: 1 1 0%;
  margin-top: 4rem;
}

.lower {
  margin-bottom: 1rem;;
}

button {
  width: 100%;
  padding-top: 1rem;
  padding-bottom: 1rem;
  border-radius: 999px;
}

</style>
