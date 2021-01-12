<template>
  <div class="Container">
    <div class="row items-start example-container">
      <div class="example-cell col-4" tabindex="0">
        <q-card
          class="my-card text-white"
          style="background: radial-gradient(circle, #35a2ff 0%, #014a88 100%)"
        >
          <q-card-section>
            <div class="text-h6">Our Changing Planet</div>
            <div class="text-subtitle2">by John Doe</div>
          </q-card-section>

          <q-card-section class="q-pt-none">
            {{ lorem }}
          </q-card-section>
        </q-card>
      </div>
      <div class="example-cell col-4" tabindex="0">
        <q-card class="my-card-two">
          <q-card-section horizontal>
            <q-img
              class="col-5"
              src="https://cdn.quasar.dev/img/parallax1.jpg"
            />

            <q-card-section>
              {{ lorem }}
            </q-card-section>
          </q-card-section>

          <q-separator />

          <q-card-actions>
            <q-btn flat round icon="event" />
            <q-btn flat>
              5:30PM
            </q-btn>
            <q-btn flat>
              7:00PM
            </q-btn>
            <q-btn flat color="primary">
              Reserve
            </q-btn>
          </q-card-actions>
        </q-card>
      </div>
    </div>
    <br/>
    <div class="left">
      <center><q-btn color="blue" icon="home" label="GO HOME" to="/" @click="$router.replace('/')"/></center>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    }
  }
}
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px

.my-card-two
  width: 100%
  max-width: 350px

.flex-break
  flex: 1 0 100% !important
  height: 0 !important

.example-container
  .example-cell
    margin: 1px
    padding: 4px 8px

</style>
