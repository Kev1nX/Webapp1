<template>
    <div class="contract">
        <!-- <h3>{{ contract.name }}</h3>
        <h4>Email: {{ contract.email}}</h4>
        <h4>Phone number: {{ contract.phone }}</h4>
        <h4>Website: {{ contract.website }}</h4>
        <h4>{{ contract.company }}</h4> -->
        <v-expansion-panels variant="popout" class="my-4">
          <v-expansion-panel>
            <v-expansion-panel-title class = "panel-title">{{ contract.name }}</v-expansion-panel-title>
                <v-expansion-panel-text>Email : {{ contract.email}}</v-expansion-panel-text>
                <v-expansion-panel-text>Phone number : {{ contract.phone }}</v-expansion-panel-text>
                <v-expansion-panel-text>Website : {{ contract.website }}</v-expansion-panel-text>
          </v-expansion-panel>
        </v-expansion-panels>
    </div>
</template>

<script>
export default{
    name :'Contract',
    props:{
        contract: Object,
    },

}
</script>
<style scoped>
.panel-title{
  font-family: Arial, Helvetica, sans-serif;
  font-size: larger;
}
.contract {
  background: #d3d2d2;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
.contract h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
h4{
  color:#000000;
}
</style>