<template>
  <q-layout view="lHh Lpr fff">
    <q-page-container>
      <q-page
        class="window-height window-width row justify-center items-center"
      >
        <div class="column q-pa-lg">
          <div class="row shadow-24 al-card">
            <q-card class="al-card" flat bordered>
              <q-card-section>
                <div class="text-h6 text-center">Productive Portal</div>
                <div class="text-subtitle2 text-center">different Modules</div>
              </q-card-section>

              <q-tabs v-model="tab" class="text-teal">
                <q-tab label="Signin" name="one" />
                <q-tab label="Signup" name="two" />
              </q-tabs>

              <q-separator />

              <q-tab-panels v-model="tab" animated>
                <q-tab-panel name="one">
                  The QCard component is a great way to display important pieces
                  of grouped content.
                </q-tab-panel>

                <q-tab-panel name="two">
                  With so much content to display at once, and often so little
                  screen real-estate, Cards have fast become the design pattern
                  of choice for many companies, including the likes of Google
                  and Twitter.
                </q-tab-panel>
              </q-tab-panels>
            </q-card>
          </div>
        </div>
      </q-page>
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    const tab = ref("one");
    return {
      tab,
    };
  },
};
</script>
