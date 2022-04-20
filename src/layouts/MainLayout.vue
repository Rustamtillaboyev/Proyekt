<template>
  <q-layout view="hHh lpR fFf">

    <q-header elevated class="bg-dark text-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <!-- <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg"> -->
            <a class="header-envato_market" href="https://themeforest.net/item/xtrm-extreme-sports-wordpress-theme/23423423">Envato Market</a>
          </q-avatar>
          envato<span class="market">market</span>
          <q-btn label="Buy now" class="bg-positive buy-now"/>
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
          </q-avatar>
          <div>Title</div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>

  </q-layout>
</template>


<style scoped>
.market{
  color: rgb(19, 178, 19);
}
.buy-now{
  margin-left: 1050px;
}

</style>
