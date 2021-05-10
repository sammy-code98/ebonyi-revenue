<template>
  <div class="row bg-img text-white q-mt-xl">
    <div class="col-xs-12 col-sm-6 col-md-4 ">
      <q-img src="~assets/logo-1.png"/>
      <div class="q-ma-md text-subtitle2">
        Ebsirs is the operational arm of the Ebonyi State Government responsible
        for the collection of taxes and other revenues.
      </div>
      <div class="text-center text-weight-bold">Follow us on</div>
      <div class="q-gutter-xs" style=" margin:auto;">
        <div class="text-center" style="margin:auto">
          <q-btn color="info" icon="mdi-twitter" flat />
          <q-btn color="primary" icon="mdi-facebook" flat />
          <q-btn color="red-6" icon="mdi-instagram" flat />
        </div>
      </div>
    </div>
    <div class="col-xs-12 col-sm-6 col-md-4   ">
      <div class="text-uppercase text-center q-ma-md text-weight-bold">
        quick links
      </div>
      <div>
        <q-list separator>
          <q-item clickable v-ripple>
            <q-item-section>Tax Information</q-item-section>
            <q-item-section side>
              <q-icon name="mdi-greater-than" color="green" />
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section>News</q-item-section>
            <q-item-section side>
              <q-icon name="mdi-greater-than" color="green" />
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section>About Us</q-item-section>
            <q-item-section side>
              <q-icon name="mdi-greater-than" color="green" />
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple>
            <q-item-section>Contact Us</q-item-section>
            <q-item-section side>
              <q-icon name="mdi-greater-than" color="green" />
            </q-item-section>
          </q-item>
        </q-list>
      </div>
    </div>
    <div class="col-xs-12 col-sm-6 col-md-4  ">
      <div class="text-uppercase text-center q-ma-md text-weight-bold">
        subscribe
      </div>
      <div class="text-center ">Stay in the know. Join our mailing list</div>
      <q-input
        color="white"
        class="q-ma-md"
        label-color="green"
        v-model="email"
        outlined
        type="email"
        label="Email"
        placeholder="example@xyz.com"
      />
      <div class="gt-sm q-pa-md">
        <q-btn
        color="positive"
        label="Submit"
        no-caps
        class="q-ma-md  full-width" 
      />
      </div>
      
      <div class="lt-md q-pa-md">
        <q-btn
          color="positive"
          label="Submit"
          no-caps
          class="q-mr-xl q-ml-xl full-width"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      email: "",
      footerLinks: [
        {
          title: "Why QuizeApp?",
          link1: "Product",
          link2: "Solutions",
          link3: "Blog",
          link4: "Shop",
          link5: "Status"
        },
        {
          title: "Resources",
          link1: "Product",
          link2: "Solutions",
          link3: "Blog",
          link4: "Shop",
          link5: "Status"
        },
        {
          title: "Community",
          link1: "Product",
          link2: "Solutions",
          link3: "Blog",
          link4: "Shop",
          link5: "Status"
        },
        {
          title: "Support",
          link1: "Product",
          link2: "Solutions",
          link3: "Blog",
          link4: "Shop",
          link5: "Status"
        },
        {
          title: "Company",
          link1: "Product",
          link2: "Solutions",
          link3: "Blog",
          link4: "Shop",
          link5: "Status"
        }
      ]
    };
  }
};
</script>
<style lang="scss" scoped>
#footer-logo {
  transform: translate(50%, -50%);
  margin: 0 auto;
}
.bg-img {
  background: linear-gradient(rgba(9, 11, 32, 0.8), rgba(24, 19, 21, 0.8));
  opacity: 0.9;
}
</style>
