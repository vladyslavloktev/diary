<template>
  <q-item class="card q-mt-sm">
    <q-item-section>
      <q-item-label>Single line item</q-item-label>
      <img class="card-img q-my-sm" src="https://cdn.quasar.dev/img/mountains.jpg">
      <q-item-label  caption lines="1">Secondary line text. Lorem ipsum dolor sit amet, consectetur adipiscit elit.</q-item-label>
    </q-item-section>

    <q-item-section side top>
      <q-item-label caption>5 min ago</q-item-label>
        <q-card-actions vertical class="justify-around q-py-md" >
        <q-btn flat round color="red" icon="create" @click="clickFav"/>
        <q-btn flat round color="accent" icon="bookmark" @click="clickSave"/>
        <q-btn flat round color="primary" icon="share" @click="clickShare"/>
      </q-card-actions>
    </q-item-section>
  </q-item>
</template>

<script>

export default {
  name: 'BookCardElement',
  methods: {
    clickSave: function () {
      return alert('save this post to favorites')
    },
    clickFav: function () {
      return alert('i answer for edit function')
    }
  }
}

</script>

<style scoped>
  .card-img {
    max-width: 58vw;
  }
</style>
