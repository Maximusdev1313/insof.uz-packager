<template>
  <div class="container">
    <div class="wrapper">
      <div class="card shadow-4">
        <div class="card_title">Yangi kategoriya qo'shish</div>
        <div class="card_fields">
          <q-input label="Kategoriya nomi" />
          <q-input label="Kategoriya uchun rasm(link)" />
        </div>
      </div>
      <!-- card for recent  -->
      <div class="recent shadow-4">
        <q-scroll-area style="height: 200px; max-width: 90%; margin: 0 auto">
          <div v-for="n in 50" :key="n" class="q-py-xs">
            Lorem ipsum dolor sit amet, consectetur adipisicing
            <q-separator />
          </div>
        </q-scroll-area>
      </div>
    </div>
  </div>
</template>

<style lang="sass" scoped>
.container
    width: 95%
    margin: 0 auto

.wrapper
    width: 100%
    margin-top: 20px
    display: flex
    justify-content: space-between
    align-items: center
    flex-wrap: wrap
.card
    width: 700px
    height: 200px
    border-radius: 20px
    display: flex
    justify-content: center
    align-items: center
    flex-direction: column
    flex-grow: 1
    margin: 10px 20px

.card_title
    text-align: center
    font-size: 20px
    font-weight: bold
    color: grey
.card_fields
    width: 70%
    margin: 0 auto

.recent
    width: 300px
    height: 200px
    border-radius: 20px
    flex-grow: 1
    margin: 10px 20px
</style>