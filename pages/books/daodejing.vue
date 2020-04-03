<template>
  <div>
    <h2 class="page-header book-name ml-5">
      О книге
    </h2>
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
        <div class="book-properties">
          <div class="book-property">
            <div class="book-property-key">
              Название книги
            </div>
            <div class="book-property-value">
              Дао дэ цзин: опыт русского перевода.<br />
              Изд. 2-е, испр. и доп.
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Автор
            </div>
            <div class="book-property-value">
              Лао Цзы
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Язык оригинала
            </div>
            <div class="book-property-value">
              Древнекитайский
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Переводчик
            </div>
            <div class="book-property-value">
              Карен Петросян<br />
              Доктор филологических наук (Dr. philol.)
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Издатель
            </div>
            <div class="book-property-value">
              Рижское общество китайских исследований
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Язык издания
            </div>
            <div class="book-property-value">
              Русский, китайский (для текста Дао дэ цзин)
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Количество страниц
            </div>
            <div class="book-property-value">
              176
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Год выпуска
            </div>
            <div class="book-property-value">
              2020
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Тип обложки
            </div>
            <div class="book-property-value">
              Мягкая обложка
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              ISBN
            </div>
            <div class="book-property-value">
              978-9934-8913-0-4
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key">
              Вес в упаковке
            </div>
            <div class="book-property-value">
              г
            </div>
          </div>
          <div class="book-property">
            <div class="book-property-key-title">
              О переводе
            </div>
          </div>
          <div class="book-property">
            Задача нашего перевода – попытаться обойтись без понятий европейской
            философии, т.е. обойтись без посредника, не применяя языка третьей культуры.
            Историческая, культурная, хозяйственно-бытовая терминология также была
            переведена с учётом многовековой традиции русской письменности. Многие
            иероглифы переводились русскими словами, давно вышедшими из употребления
            как в письменной, так и в устной речи. Достаточно упомянуть такие слова как
            «воевода», «завоеводчик», «вежа», «гудьба» и др. Таким образом, как громко бы
            это ни звучало, но новизна нашего перевода именно в том, что можно назвать
            первым русским экспериментальным переводом, что и отразилось в названии
            данной книги.
          </div>
          <div class="book-property">
            <div class="book-property-key-title">
              О содержании книги
            </div>
          </div>
          <div class="book-property">
            Помимо самого перевода, для удобного изучения оригинального текста ДДЦ, мы
            дали китайский текст (с русской тональной транскрипцией), привели наиболее
            важные разночтения между списками ДДЦ. В приложении имеется
            иероглифический указатель.
          </div>
          <div class="book-property">
            <div class="book-property-key-title">
              Приобрести книгу
            </div>
          </div>
          <div class="book-property">
            <span>
              По вопросам приобретения книги обращайтесь по электронному адресу:
              <a href="mailto:info@daodejing.eu">info@daodejing.eu</a>
            </span>
            <form
              action="https://www.paypal.com/cgi-bin/webscr"
              method="post"
              target="_top"
            >
              <input type="hidden" name="cmd" value="_s-xclick" />
              <input type="hidden" name="hosted_button_id" value="THFFX92ZQJL3S" />
              <input
                type="image"
                src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif"
                border="0"
                name="submit"
                title="PayPal - The safer, easier way to pay online!"
                alt="Donate with PayPal button"
              />
              <img
                src="https://www.paypal.com/en_LV/i/scr/pixel.gif"
                alt=""
                border="0"
                width="1"
                height="1"
              />
            </form>

          </div>
        </div>
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
.book-properties {
  display: flex;
  flex-direction: column;
}

.book-property {
  display: flex;
  flex-direction: row;
  margin-bottom: 1em;
}

.book-property-key {
  flex-basis: 150px;
  flex-shrink: 0;
  flex-grow: 0;
  margin-right: 10px;
}

.book-property-key-title {
  font-weight: bold;
}

.book-property-value {
  flex-shrink: 1;
  flex-grow: 1;
}
</style>
