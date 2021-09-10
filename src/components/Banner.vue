<template>
  <div class="q-mt-xl">
    <q-img src="~assets/building.jpg" height="680px">
      <div class="absolute-full text-subtitle2 inline-flex text-center">
        <div :class="$q.screen.lt.md ? 'text-h4  text-weight-bold ' : 'text-h3  text-weight-bold ' " id="banner-text">
          Efficient and Transparent Processes
        </div>
        <div class="q-mt-md text-body1 text-weight-regular q-pa-xl" :class="$q.screen.lt.md ? 'q-mt-sm   text-caption text-weight-bold' : 'q-mt-md text-body1 text-weight-regular' " >
          Ebonyi State moves towards meeting the needs of a mega city, Ebsirs
          continues to position itself as the major funding arm of the state
          government by putting in place structures that will ensure collection
          of the proper amount of tax revenue at the least cost.
        </div>
        <q-btn
          color="positive"
          label="What We Do"
          icon-right="mdi-arrow-right"
          no-caps
          dense
          class="q-pa-sm q-mt-md"
        />
      </div>
    </q-img>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  }
};
</script>
<style scoped>
#banner-text{
  margin-top: 270px;
}
</style>
