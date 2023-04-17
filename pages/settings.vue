<template>
  <div>
    <div class="page-intro">
      <div class="container-fluid padding-top-2">
        <div class="page-intro__header">
          <h1 class="page-intro__heading main-heading">
            Настройки
          </h1>
        </div>
      </div>
    </div>
    <div class="container-fluid padding-top-2">
      <div class="setting-section">
        <sip-call />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import {Component} from "nuxt-property-decorator";
import SipCall from "~/components/setting-section/SipCall.vue";

@Component({
  components: {SipCall}
})
export default class Settings extends Vue{

}
</script>

<style lang="scss" scoped>
.page-intro{
  background: #f9f9fc;
  padding: 0 0 0.1rem;

  &__header{
    -webkit-box-align: center;
    -moz-box-align: center;
    -ms-flex-align: center;
    -webkit-align-items: center;
    align-items: center;
    display: -webkit-box;
    display: -webkit-flex;
    display: -moz-box;
    display: -ms-flexbox;
    display: flex;
    margin-bottom: 1.5rem;
  }
}
.container-fluid{
  margin: 0 auto;
  max-width: 1920px;
  padding: 0 1.5rem;
}

.main-heading{
  color: #000;
  font-family: Montserrat,Helvetica,Arial,sans-serif;
  font-size: 2.6rem;
  font-weight: 600;
  line-height: 1.25;
  margin-bottom: 1.5rem;
}

.padding-top-2{
  padding-top: 2rem;
}
</style>
