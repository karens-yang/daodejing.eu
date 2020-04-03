<template>
  <div>
    <h2 class="page-header book-name ml-5">
      Контакты
    </h2>

    <v-card
      class="mx-auto"
      max-width="400"
      outlined
    >
      <v-list-item three-line>
        <v-list-item-content>
          <div class="overline mb-4">
            Рижское общество <br />китайских исследований
          </div>
          <v-list-item-subtitle>
            <v-icon small class="mr-1 mb-1">
              mdi-badge-account-horizontal-outline
            </v-icon>
            Регистрационный номер:
          </v-list-item-subtitle>
          <v-list-item-title>
            <span>40008293937</span>
          </v-list-item-title>
        </v-list-item-content>
        <v-list-item-avatar
          tile
          size="80"
          color="white"
        >
          <img src="/img/logo.png" />
        </v-list-item-avatar>
      </v-list-item>
      <v-list-item style="margin-top: -17px;">
        <v-list-item-content>
          <v-list-item-subtitle>
            <v-icon small class="mr-1">
              mdi-home-outline
            </v-icon>
            Юридический адрес:
          </v-list-item-subtitle>
          <v-list-item-title class="mb-2">
            Zolitudes 46/1-34, Rīga LV-1029, Latvia.
          </v-list-item-title>
          <v-list-item-subtitle>
            <v-icon small class="mr-1">
              mdi-email
            </v-icon>
            Электронная почта:
          </v-list-item-subtitle>
          <v-list-item-title class="mb-1">
            info@daodejing.eu
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-card>

    <br />

    <v-card
      class="mx-auto"
      max-width="400"
      outlined
    >
      <v-list-item three-line>
        <v-list-item-content>
          <div class="overline mb-4">
            Рижское общество <br />китайских исследований
          </div>
          <v-list-item-subtitle>
            <v-icon small class="mr-1 mb-1">
              mdi-gift-outline
            </v-icon>
            Поддержать сообщество:
          </v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-avatar
          tile
          size="80"
          color="white"
        >
          <img src="/img/logo.png" />
        </v-list-item-avatar>
      </v-list-item>

      <br />
      <form
        style="text-align: center;"
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

      <br />

      <div style="text-align: center;">
        <div>или с телефона</div>
        <br />
        <div style="text-align: center;">
          <img height="256" weight="256" src="/img/donate-qr.png" />
        </div>
      </div>

      <br />
      <br />
    </v-card>

  </div>
</template>
