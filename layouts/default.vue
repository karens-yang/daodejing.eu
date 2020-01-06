<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <!--      <v-btn @click.stop="miniVariant = !miniVariant" icon>-->
      <!--        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>-->
      <!--      </v-btn>-->
      <!--      <v-btn @click.stop="clipped = !clipped" icon>-->
      <!--        <v-icon>mdi-application</v-icon>-->
      <!--      </v-btn>-->
      <!--      <v-btn @click.stop="fixed = !fixed" icon>-->
      <!--        <v-icon>mdi-minus</v-icon>-->
      <!--      </v-btn>-->
      <img
        src="img/logo.png"
        alt="logo"
        width="48px"
        height="48px"
        style="margin-left:5px; margin-right: 15px;"
      />
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <!--      <v-btn @click.stop="rightDrawer = !rightDrawer" icon>-->
      <!--        <v-icon>mdi-menu</v-icon>-->
      <!--      </v-btn>-->
    </v-app-bar>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
    <!--    <v-navigation-drawer v-model="rightDrawer" :right="right" temporary fixed>-->
    <!--      <v-list>-->
    <!--        <v-list-item @click.native="right = !right">-->
    <!--          <v-list-item-action>-->
    <!--            <v-icon light>-->
    <!--              mdi-repeat-->
    <!--            </v-icon>-->
    <!--          </v-list-item-action>-->
    <!--          <v-list-item-title>Switch drawer (click me)</v-list-item-title>-->
    <!--        </v-list-item>-->
    <!--      </v-list>-->
    <!--    </v-navigation-drawer>-->
    <v-footer :fixed="fixed" app>
      <img
        src="img/logo.png"
        alt="logo"
        width="24px"
        height="24px"
        style="margin-right: 10px;"
      />
      <span>Rīgas biedrība Ķīnas pētniecībai &copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        {
          icon: 'mdi-home',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-book-open-variant',
          title: 'About the Book',
          to: '/inspire'
        },
        {
          icon: 'mdi-email',
          title: 'Contacts',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'RĪGAS BIEDRĪBA ĶĪNAS PĒTNIECĪBAI'
    }
  }
}
</script>
