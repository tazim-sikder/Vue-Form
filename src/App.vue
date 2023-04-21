<template>
  <v-app>
    <v-main>
      <h1>Voice Provisioning</h1>
      <v-sheet width="1170" class="mx-auto">
      <v-form>
        <v-sheet height="91" >
        <v-select
          label="Select a Partner"
          :items="['Sprout', 'Sprout']"
          bg-color="blue-lighten-5"
          variant="solo"
        ></v-select>
        </v-sheet>

        <v-sheet height="91" >
        <v-text-field
          label="Account Number"
          color="black"
          bg-color="blue-lighten-5"
          variant="solo"
        ></v-text-field>
        </v-sheet>

        <div class="d-flex justify-space-between flex-row">
        <v-sheet width="565" height="91" >
          <v-text-field
            label="First Name"
            color="black"
            bg-color="blue-lighten-5"
            class="rounded-lg"
            variant="solo"
            type="input"
          ></v-text-field>
          </v-sheet>
        <v-sheet width="565" height="91" >
          <v-text-field
            label="Last Name"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
            type="input"
          ></v-text-field>
          </v-sheet>
        </div>

        <div class="d-flex justify-space-between flex-row">
        <v-sheet width="275" height="91" >
          <v-text-field
            label="Address"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        <v-sheet width="275" height="91" >
          <v-text-field
            label="City"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        <v-sheet width="275" height="91" >
          <v-text-field
            label="State"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        <v-sheet width="275" height="91" >
          <v-text-field
            label="Zip"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        </div>

        <div class="d-flex justify-space-between flex-row">
        <v-sheet width="565" height="91" >
          <v-text-field
            label="Contact Phone"
            type="tel"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        <v-sheet width="565" height="91" >
          <v-text-field
            label="Contact Email"
            type="email"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        </div>

        <div class="d-flex justify-space-between flex-row">
          <v-sheet width="370" height="91" >
          <v-select
          label="Customer Type"
          :items="['', '']"
          bg-color="blue-lighten-5"
          variant="solo"
        ></v-select>
            </v-sheet>
        <v-sheet width="370" height="91" >
          <v-text-field
            label="Phone Number to Provision"
            type="tel"
            color="black"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        <v-sheet width="370" height="91" >
          <v-text-field
            label="Sip Password"
            type="email"
            bg-color="blue-lighten-5"
            variant="solo"
          ></v-text-field>
          </v-sheet>
        </div>

        <v-sheet width="370" height="91" >
          <v-select
          label="Ported"
          :items="['', '']"
          bg-color="blue-lighten-5"
          variant="solo"
        ></v-select>

        </v-sheet>
       


        <div class="d-flex flex-row">
          <v-checkbox label="Bypass E911 Address Automation"></v-checkbox>

        <v-sheet width="775" height="91" >
          <v-alert
            variant="outlined"
            type="warning"
            prominent
            border="top"
          >
            (By checking "Bypass E911 Address Automation" you agree to manually
            add this phone number and address to Bandwidth)
          </v-alert>
          </v-sheet>
        </div>

        <v-sheet width="120" height="91" >
        <v-btn
          type="submit"
          block
          class="mt-2"
          color="deep-purple-darken-4"
          >Provision</v-btn
        >
        </v-sheet>
      </v-form>
      </v-sheet>
    </v-main>
  </v-app>
</template>

<script setup></script>
<style>
  h1 {
    text-align: center;
  }
</style>
