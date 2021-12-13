<template>
  <a-layout-header :style="{ width: '100%', display: 'flex', justifyContent: 'space-between'  }">
    <h2 class="logo">
      THE MOVIE DB
    </h2>
    <a-dropdown class="main-dd" :trigger="['click']">
      <a class="ant-dropdown-link" @click="e => e.preventDefault()">
        <a-avatar icon="user" />
        Click me <a-icon type="down" />
      </a>
      <a-menu slot="overlay">
        <a-menu-item key="0">
          <a href="#">1st menu item</a>
        </a-menu-item>
        <a-menu-item key="1">
          <a href="#">2nd menu item</a>
        </a-menu-item>
        <a-menu-divider />
        <a-menu-item key="3">
          3rd menu item
        </a-menu-item>
      </a-menu>
    </a-dropdown>
  </a-layout-header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      collapsed: false,
    };
  },
}
</script>

<style>

.main-dd {
  color: white;
}
.logo {
  color: white;
}
</style>
