<template>
  <div>
    <div></div>
    <q-carousel
      animated
      :autoplay="autoplay"
      v-model="slide"
      navigation
      infinite
      class="img-overlay"
    >
      <q-carousel-slide :name="1" img-src="~assets/dave.jpg" class="img">
        <div :class="$q.screen.lt.md ? 'q-ma-md' : 'q-mt-xl  text-center'">
          <div :class="$q.screen.lt.md ? 'text-h4 ' : 'text-h2 '">
            Pay your tax and lets grow together!!!
          </div>
          <div
            :class="
              $q.screen.lt.md
                ? 'text-subtitle1'
                : 'text-body1  q-mt-md text-weight-regular'
            "
          >
            As Ebonyi State moves towards meeting the needs of a mega city ,
            Ebsirs continues to position itself as the major funding arm
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

      <q-carousel-slide :name="2" img-src="~assets/camp.jpg" class="img">
        <div :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div :class="$q.screen.lt.md ? 'text-h4' : 'text-h2'">
            Pay your tax and lets grow together!!!
          </div>
          <div
            :class="
              $q.screen.lt.md
                ? 'text-subtitle1'
                : 'text-body1  q-mt-md text-weight-bold'
            "
          >
            As Ebonyi State moves towards meeting the needs of a mega city ,
            Ebsirs continues to position itself as the major funding arm
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
      <q-carousel-slide :name="3" img-src="~assets/building.jpg" class="img">
        <div :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div :class="$q.screen.lt.md ? 'text-h4 ' : 'text-h2'">
            Pay your tax and lets grow together!!!
          </div>
          <div
            :class="
              $q.screen.lt.md
                ? 'text-subtitle1'
                : 'text-body1  q-mt-md text-weight-bold'
            "
          >
            As Ebonyi State moves towards meeting the needs of a mega city ,
            Ebsirs continues to position itself as the major funding arm
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
      <q-carousel-slide :name="4" img-src="~assets/building.jpg" class="img">
        <div :class="$q.screen.lt.md ? 'q-ma-md  ' : 'absolute-center'">
          <div :class="$q.screen.lt.md ? 'text-h4' : 'text-h2'">
            Pay your tax and lets grow together!!!
          </div>
          <div
            :class="
              $q.screen.lt.md
                ? 'text-subtitle1'
                : 'text-body1  q-mt-md text-weight-bold'
            "
          >
            As Ebonyi State moves towards meeting the needs of a mega city ,
            Ebsirs continues to position itself as the major funding arm
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
      slide: 1,
      autoplay:true
    };
  }
};
</script>

<style lang="scss" scoped>
.img-overlay {
  overflow: hidden;
  color:#fff;
  text-align: center;
  background: black;
  background: linear-gradient(rgba(9, 11, 32, 0.8), rgba(24, 19, 21, 0.8));
  opacity: 0.8;
}

.img {
  object-fit: contain;
  opacity: 0.6;
}
</style>
