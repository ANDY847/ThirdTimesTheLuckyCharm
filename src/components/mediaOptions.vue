<template>
  <!----flex center trys to make item in center of container------>
  <q-page>
    <!----------------------tooolbar--------------->
    <div class="q-pa-md q-gutter-x-xs q-gutter-y-lg">
      <q-toolbar class="bg-light-blue text-white shadow-2">
        <q-btn flat round dense icon="menu" class="q-mr-sm"/>
        <q-space/>
        <q-btn-toggle
          v-model="model"
          flat
          stretch
          toggle-color="purple"
          :options="[
          {label: 'Details', value: 'one'},
          {label: 'Media', value: 'two'},
          {label: 'Open To', value: 'three'}
        ]"
        />
      </q-toolbar>
    </div>

    <!----------------------tooolbar--------------->
    <div class="row inline col">
      <q-card v-for="n in 20" :key="n">
        <div class="col-auto q-ma-sm">
          <img
            alt="Louis so cute"
            style="max-height: 150px; max-width: 100px"
            src="~assets/IMG_4455.jpg"
          >
          add some details
        </div>
      </q-card>
    </div>
  </q-page>
</template>

<style></style>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
      model: "one"
    };
  },
  methods: {
    onItemClick() {
      console.log("Clicked on an Item");
    }
  }
};
</script>
