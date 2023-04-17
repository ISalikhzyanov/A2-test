<template>
  <div class="wide-section setting-section__subsection">
    <div>
      <div>Звонки через SIP</div>
      <div>
        <v-switch
          v-model="model"
        ></v-switch>
      </div>
    </div>
    <div>
      <div>
        <p>
          Включите эту функцию чтобы Авито и другие площадки не блокировали ваш аккаунт. Будет выглядеть так, будто звонки совершаются с разных номеров.
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">

import {Component} from "nuxt-property-decorator";
import Vue, {ref} from "vue";

@Component
export default class SipCall extends Vue{
  model: boolean = false
}
</script>

<style lang="scss" scoped>

</style>

