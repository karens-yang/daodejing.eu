<template>
  <div>
    <h2 class="page-header book-name ml-5">Дао Дэ Цзин опыт русского перевода</h2>
    <v-card class="mb-4 front-image ml-5 mt-4" max-width="540px">
      <v-img
        src="/img/cover.jpg"
        alt="Книга «Дао Дэ Цзин: опыт русского перевода»"
        width="540"
        contain="true"
        class="grey darken-4"
        style="background-color: white;"
      ></v-img>
      <v-card-text>
        Книга «Дао Дэ Цзин:<br />Опыт русского перевода»
      </v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'Книга «Дао Дэ Цзин: опыт русского перевода»'
    }
  }
}
</script>

<style>
.page-header.book-name {

}
</style>
