<template>
  <v-row>
    <v-col class="text-center">
      <img
        src="/v.png"
        alt="Vuetify.js"
        class="mb-5"
      >
      <blockquote class="blockquote">
        &#8220;First, solve the problem. Then, write the code.&#8221;
        <footer>
          <small>
            <em>&mdash;John Johnson</em>
          </small>
        </footer>
      </blockquote>
    </v-col>
    <v-switch
      v-model="switch1"
      :label="`Switch 1: ${switch1.toString()}`"
    ></v-switch>
  </v-row>
</template>

<script>
export default {
  name: 'InspirePage',
  data () {
    return {
      switch1: true
    }
  }
}
</script>
