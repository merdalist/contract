<template>
<v-form>
  <v-row justify="center" align="center">
    <v-col cols="12"
      sm="10"
      md="8"
      lg="6">
      <v-card class="logo py-4 d-flex justify-center">
        <v-img
        height="300"
        src="https://www.curt.org/wp-content/uploads/2019/12/iStock-1019006292-1280x854.jpg"
        ></v-img>
      </v-card>
      <v-card ref="form">
        <v-card-title class="justify-center" style="font-size:2em" >Contractor Form</v-card-title>
        <v-card-text>
          <v-text-field
            ref="name"
            v-model="first"
            label="ETH Price"
            readonly
          ></v-text-field>
          <v-text-field
            ref="address"
            v-model="second"
            label="ETH Blocked"
            readonly
            ></v-text-field>
          <v-text-field
            ref="city"
            v-model="third"
            label="Project Cost (ETH)"
            readonly
            ></v-text-field>
          <v-text-field
            ref="state"
            v-model="fourth"
            label="Project Cost"
            readonly
            ></v-text-field>
          <v-text-field
            ref="zip"
            v-model="fifth"
            label="Contractor Public Key"
            readonly
            ></v-text-field>
         </v-card-text>
         <v-card-actions>
         <div class="my-2">
          <v-btn
          color="primary"
          light
          background-color="yellow">
            Project Start
          </v-btn>
          </div>
          <v-spacer></v-spacer>
          <v-btn
            color="orange"
            light
            bold
            @click="submit"
          >
            Submit
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
 </v-form>
</template>

<script>
  export default {
    data: () => ({
      first: "$ 3200",
      second: "$ 3200",
      third: "$ 0,85",
      fourth: "$ 2000",
      fifth: "0x000056469456434861534414"
    }),
}
</script>