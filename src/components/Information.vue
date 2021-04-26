<template>
  <div class="row q-pa-xl">
    <div class="col-xs-12 col-sm-6 col-md-6 q-pa-md ">
      <q-img src="~assets/dave.jpg" height="400px" class="rounded-borders">
        <div class="absolute-center flex flex-center">
          <q-icon
            name="mdi-newspaper"
            class="text-white absolute-left"
            style="font-size: 4.4em;"
          />

          <div class="q-pt-xl q-ma-md text-h5">
            Visit our newsfeed to stay updated
          </div>
        </div>
      </q-img>
    </div>
    <div class="col-xs-12 col-sm-6 col-md-6 q-pa-md  ">
      <q-img src="~assets/building.jpg" height="400px" class="rounded-borders">
        <div class="absolute-center flex flex-center">
          <q-icon
            name="mdi-map-marker-multiple"
            class="text-white absolute-left"
            style="font-size: 4.4em;"
          />

          <div class="q-pt-xl q-ma-md text-h5">
            Find our Tax stations around Ebonyi
          </div>
        </div>
      </q-img>
    </div>

    <div
      class="col-xs-12 col-sm-12 col-md-4 q-pa-md q-mt-xl"
      v-for="(info, index) in informations"
      :key="index"
    >
      <q-card dark bordered class="bg-green-5 my-card">
        <q-card-section>
          <q-icon
          :name="info.icon"
            class="text-white absolute-center q-mt-lg "
            style="font-size: 4.4em;"
          />

        </q-card-section>

        <q-card-section class="text-h6 text-center q-mt-xl text-capitalize">
          {{info.title}}
        </q-card-section>

        <q-card-section class="text-body1 text-center q-mt-md">
          {{ info.describtion }}
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      informations: [
        {
          icon: "mdi-credit-card-multiple-outline",
          title: "pay tax",
          describtion: "Make payments of All kinds of Tax HERE"
        },
        {
          icon: "mdi-google-maps",
          title: "Our Address",
          describtion:
            "The Good Shepherd Building,Block H,Plot H1Central Business DistrictOpp.Lagos State Secretariat Main Gate Alausa,Ikeja."
        },
        {
          icon: "mdi-card-account-mail",
          title: "Contact Us",
          describtion: "info@lirs.gov.ng,0700-2255-5477Monday - Friday8am - 5pm"
        }
      ],
      
    };
  }
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
  height:350px
</style>
