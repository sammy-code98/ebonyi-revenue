<template>
  <div class="q-pt-md">
    <div class="text-h3 text-center text-weight-light text-grey q-mt-xl" :class="$q.screen.lt.md ? 'text-h5 text-center text-weight-light text-grey q-mt-xl' : 'text-h3 text-center text-weight-light text-grey q-mt-xl'">
      Services that makes the process easier
    </div>

    <div class="text-center q-mt-md text-weight-light text-h6 " :class="$q.screen.lt.md ? 'text-center q-ma-md text-weight-light text-subtitle1' : 'text-center q-mt-md text-weight-light text-h6'">
      Getting information for filing your taxes just got easier
    </div>
    <div class="row items-center q-px-xl  q-mb-md">
      <div
        v-for="(service, index) in services"
        :key="index"
        class="col-xs-12 col-sm-6 col-md-3 q-pa-md q-mt-md"
      >
        <q-card
          class="my-card text-white bg-green-6"

        >
          <q-card-section> 
            <q-icon
              :name="service.icon"
              class="text-white icon-center "
              style="font-size: 4.4em;"
            />
            <div class="text-capitalize text-center text-h6">{{ service.title }}</div>
          </q-card-section>

          <q-card-section class="q-pt-none">
            {{ service.description }}
          </q-card-section>

          <q-card-actions vertical>
            <q-btn flat no-caps icon-right="mdi-arrow-right">Learn More</q-btn>
          </q-card-actions>
        </q-card>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      services: [
        {
          title: "tax type",
          icon: "mdi-folder-multiple",
          description:
            "Defines the various types of tax  collected by the  different  taxaction bodies"
        },
        {
          title: "tax systems",
          icon: "mdi-finance",
          description: "Describes the method of Tax Administration which could be Proportional, Progressive or Regressive"
        },
        {
          title: "tax collection",
          icon: "mdi-hand-water",
          description: "Tax Collection is the implementation  of measures(Tax  Policies and  Tax Laws) put in place  by a statutory government institution  for the purpose of generating and aggregating revenue for the Government"
        },
        {
          title: "tax legislation",
          icon: "mdi-library",
          description: "Tax legislation  are the acts governing  Taxation  in   Nigeria for various tax types"
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
.my-card{
  width: 100%;
  max-width: 350px;
  height: 350px;
}
.icon-center{
  margin-left: 110px ;
  margin-right: 110px;
}
</style>
