<template>
  <f7-page class="color-theme-red">
    <f7-navbar title="Izquierda Panel"></f7-navbar>
    <f7-block strong>
      <p>Left panel content goes aqui</p>
    </f7-block>
    <f7-block-title>Load page in panel</f7-block-title>
    <f7-list>
      <f7-list-item link="/about/" title="About"></f7-list-item>
      <f7-list-item link="/form/" title="Form"></f7-list-item>
    </f7-list>
    <f7-block-title>Load page in main view</f7-block-title>
    <f7-list>
      <f7-list-item link="/about/" title="About" view="#main-view" panel-close></f7-list-item>
      <f7-list-item link="/panel-left/" title="Form" view="#main-view" panel-close></f7-list-item>
      <f7-link href="/panel-left/"  view="#main-view">Nuevo</f7-link>
    </f7-list>
  </f7-page>
</template>
<script>
import routes from '../routes.js'
export default {
   data() {
    return {
    
        routes: routes,
      }
    }
  }

</script>