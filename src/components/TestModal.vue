<template>
    <ion-modal :is-open="isOpen">
      <ion-content :scollY="false">
        <div id="container">
          <h1>Heading</h1>
          <div class="continer2">
            <h2>Write a public review</h2>
            <p>Ready to create an app?</p>
            <ion-textarea label="textarea" fill="outline" placeholder="Insert text here" maxlength="4000"  :counter="true" rows="6" label-placement="stacked"></ion-textarea>
          </div>
          <div class="lower">
            <button>Start</button>
          </div>
        </div>
        </ion-content>
      </ion-modal>
</template>

<script>
import { IonContent, IonTextarea, IonModal } from '@ionic/vue';

export default {
  name: "HomePage",
  props: ['isOpen'],
  components: {
    IonContent,
    IonTextarea,
    IonModal

  },
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
