<template>
  <div class="row">
    <div class="col-xs-12 col-sm-6 col-md-6 q-pa-md">
      <q-img
        src="~assets/dave.jpg"
        height="400px"
        class="rounded-borders q-ml-sm"
      >
        <div class="absolute-full ">
          <q-icon
            name="mdi-newspaper"
            class="text-white absolute-left q-ma-md"
            style="font-size: 4.4em;"
          />

          <div class="q-pt-xl q-ma-md text-h5 text-center text-margin">
            Visit our newsfeed to stay updated
          </div>
          <p class="text-subtitle1 text-center q-pa-md">Get the best news about tax and related stuff first hand as they happen right at your finger tips</p>
        </div>
      </q-img>
    </div>
    <div class="col-xs-12 col-sm-6 col-md-6 q-pa-md  ">
      <q-img
        src="~assets/building.jpg"
        height="400px"
        class="rounded-borders q-ml-sm"
      >
        <div class="absolute-full">
          <q-icon
            name="mdi-map-marker-multiple"
            class="text-white absolute-left q-ma-md"
            style="font-size: 4.4em;"
          />

          <div class="q-pt-xl q-ma-md text-h5 text-center text-margin">
            Find our Tax stations around Ebonyi
          </div>
          <p class="text-subtitle1 text-center q-pa-md">Having troubles locating the nearest  station around you to pay your tax? No worries as we got you covered.</p>
        </div>
      </q-img>
    </div>

    <div
      class="col-xs-12 col-sm-4 col-md-4" id="large-pad"  
      v-for="(info, index) in informations"
      :key="index"
    >
      <q-card dark bordered class="bg-green-5 my-card  shadow-8">
        <q-card-section>
          <q-icon
            :name="info.icon"
            class="text-white absolute-center q-mt-lg "
            style="font-size: 4.4em;"
          />
        </q-card-section>

        <q-card-section class="text-h6 text-center q-mt-xl text-capitalize">
          {{ info.title }}
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
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.my-card {
  width: 100%;
  max-width: 300px;
  height: 350px;
  margin: 30px;
}

.text-margin {
  margin-top: 100px;
}
// media queries
@media screen and (min-width: 480px){
  #large-pad{
    padding: 40px;
  }
}
</style>
