<template>
  <div class="home">
    <Header/>
    <heroSlider/>
    <PartnerSlider/>
    <About/>
    <StoreBanner/>
    <StoreProducts/>
    <button
      class="snipcart-add-item"
      data-item-id="2"
      data-item-name="Bacon"
      data-item-price="3.00"
      data-item-weight="20"
      data-item-url="http://myapp.com/products/bacon"
      data-item-description="Some fresh bacon"
    >Buy bacon</button>
    <form
      action="https://send.pageclip.co/z5cyTLSpCQkajtu0I12L8QuHsneqeLhC/contact-form"
      class="pageclip-form"
      method="post"
    >
      <!-- Replace these inputs with your own. Make sure they have a "name" attribute! -->

      <!-- It looks like you are creating a contact form. These email and subject fields are special -->
      <!-- See https://pageclip.co/docs#special-fields for more info -->
      <input type="email" name="email" value="roscoe@example.com">
      <input type="text" name="subject" value="A contact subject">

      <!-- This button will have a loading spinner. Keep the inner span for best results. -->
      <button type="submit" class="pageclip-form__submit">
        <span>Send</span>
      </button>
    </form>
    <ResultsSlider/>
    <Calendar/>
    <Contact/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";
import HeroSlider from "@/components/HeroSlider.vue";
import PartnerSlider from "@/components/PartnerSlider.vue";
import About from "@/components/About.vue";
import StoreBanner from "@/components/StoreBanner.vue";
import StoreProducts from "@/components/StoreProducts.vue";
import ResultsSlider from "@/components/ResultsSlider.vue";
import Calendar from "@/components/Calendar.vue";
import Contact from "@/components/Contact.vue";
export default {
  name: "home",
  components: {
    Header,
    HeroSlider,
    PartnerSlider,
    About,
    StoreBanner,
    StoreProducts,
    ResultsSlider,
    Calendar,
    Contact,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>
