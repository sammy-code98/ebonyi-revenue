<template>
  <div>
    <q-carousel animated v-model="slide" navigation infinite>
      <q-carousel-slide
        :name="1"
        img-src="~assets/dave.jpg"
      >
        <div  :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div  :class="$q.screen.lt.md ? 'text-h4  text-grey-6 text-center' : 'text-h2 text-grey-2'">
            Pay your tax and lets grow together!!!
          </div>
          <div :class="$q.screen.lt.md ? 'text-subtitle1':'text-body1 text-grey-8 q-mt-md text-weight-bold'">
           As Ebonyi State  moves towards meeting the needs of a mega  city , Ebsirs  continues  to position  itself as the major funding arm
          </div>
          <div class="q-pa-md q-gutter-md">
            <q-btn
              color="positive"
              label="More Details"
              no-caps
              dense
              class="q-pa-sm"
            />
            <q-btn
              color="positive"
              label="Pay Your Taxes"
              no-caps
              dense
              class="q-pa-sm"
            />
          </div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        :name="2"
        img-src="~assets/camp.jpg"
      >
        <div  :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div  :class="$q.screen.lt.md ? 'text-h4  text-grey-6 text-center' : 'text-h2 text-grey-2'">
            Pay your tax and lets grow together!!!
          </div>
          <div :class="$q.screen.lt.md ? 'text-subtitle1':'text-body1 text-grey-8 q-mt-md text-weight-bold'">
           As Ebonyi State  moves towards meeting the needs of a mega  city , Ebsirs  continues  to position  itself as the major funding arm
          </div>
          <div class="q-pa-md q-gutter-md">
            <q-btn
              color="positive"
              label="More Details"
              no-caps
              dense
              class="q-pa-sm"
            />
            <q-btn
              color="positive"
              label="Pay Your Taxes"
              no-caps
              dense
              class="q-pa-sm"
            />
        </div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        :name="3"
        img-src="~assets/building.jpg"
      >
        <div  :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div  :class="$q.screen.lt.md ? 'text-h4  text-grey-6 text-center' : 'text-h2 text-grey-2'">
            Pay your tax and lets grow together!!!
          </div>
          <div :class="$q.screen.lt.md ? 'text-subtitle1':'text-body1 text-grey-8 q-mt-md text-weight-bold'">
           As Ebonyi State  moves towards meeting the needs of a mega  city , Ebsirs  continues  to position  itself as the major funding arm
          </div>
          <div class="q-pa-md q-gutter-md">
            <q-btn
              color="positive"
              label="More Details"
              no-caps
              dense
              class="q-pa-sm"
            />
            <q-btn
              color="positive"
              label="Pay Your Taxes"
              no-caps
              dense
              class="q-pa-sm"
            />
          </div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        :name="4"
        img-src="~assets/building.jpg"
      >
        <div  :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div  :class="$q.screen.lt.md ? 'text-h4  text-grey-6 text-center' : 'text-h2 text-grey-2'">
            Pay your tax and lets grow together!!!
          </div>
          <div :class="$q.screen.lt.md ? 'text-subtitle1':'text-body1 text-grey-8 q-mt-md text-weight-bold'">
           As Ebonyi State  moves towards meeting the needs of a mega  city , Ebsirs  continues  to position  itself as the major funding arm
          </div>
          <div class="q-pa-md q-gutter-md">
            <q-btn
              color="positive"
              label="More Details"
              no-caps
              dense
              class="q-pa-sm"
            />
            <q-btn
              color="positive"
              label="Pay Your Taxes"
              no-caps
              dense
              class="q-pa-sm"
            />
          </div>
        </div>
      </q-carousel-slide>
      
    </q-carousel>
  </div>
</template>
<script>
export default {
  data() {
    return {
      slide: 1
    };
  }
};
</script>
