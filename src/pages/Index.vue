<template>
  <q-page>
    <carousel></carousel>
    <service></service>
    <banner></banner>
    <partner></partner>
    <q-separator />
    <information></information>
    <foot></foot>
  </q-page>
</template>

<script>
import carousel from "src/components/Carousel";
import service from "src/components/Services";
import banner from "src/components/Banner";
import partner from "src/components/Partners";
import information from "src/components/Information";
import foot from "src/components/Footer"

export default {
  name: "PageIndex",
  components: {
    carousel,
    service,
    banner,
    partner,
    information,
    foot
    
  }
};
</script>
