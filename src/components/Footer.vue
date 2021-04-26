<template>
   

     
  <div class="row bg-white text-green-5 ">
      <div class="col q-ma-md">
                <q-img src="~assets/logo-1.png"/>
                        <div class="q-ma-md text-subtitle2">Ebsirs is the operational arm of the Ebonyi State Government responsible for the collection of taxes and other revenues.</div>
        <div class="text-center text-weight-bold">Follow us on</div>
        <div class="q-gutter-xs" style=" margin:auto;">
        <div class="text-center" style="margin:auto">
          <q-btn color="info" icon="mdi-twitter" flat />
          <q-btn color="primary" icon="mdi-facebook" flat />
          <q-btn color="red-6" icon="mdi-instagram" flat />
        </div>
    </div>


      </div>
      <div class="col">
        <div class="text-uppercase text-center q-ma-md text-weight-bold">quick links</div>
        <div>
            <q-list  separator>
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
      <div class="col">
          <div  class="text-uppercase text-center q-ma-md text-weight-bold">subscribe</div>
          <div class="text-center ">Stay in the know. Join our mailing list</div>
                <q-input color="teal" class="q-ma-md" v-model="email"   outlined type="email" placeholder="Your E-mail Address"/>
    <q-btn color="positive" icon-right="mdi-arrow-right" label="Submit" no-caps  class="q-ma-md"/>

      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
        email:'',
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
  margin: 0  auto;
}
</style>
