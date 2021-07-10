<template>
  <div class="top-bar">
    <b-nav pills>
      <b-nav-item-dropdown
      id="my-nav-dropdown"
      text="EN"
      toggle-class="nav-link-custom"
      right
    >
      <b-dropdown-item>One</b-dropdown-item>
      <b-dropdown-item>Two</b-dropdown-item>
      <b-dropdown-divider></b-dropdown-divider>
      <b-dropdown-item>Three</b-dropdown-item>
      </b-nav-item-dropdown>
      <b-nav-item-dropdown
        id="my-nav-dropdown"
        text="EUR"
        toggle-class="nav-link-custom"
        right
      >
        <b-dropdown-item>One</b-dropdown-item>
        <b-dropdown-item>Two</b-dropdown-item>
        <b-dropdown-divider></b-dropdown-divider>
        <b-dropdown-item>Three</b-dropdown-item>
      </b-nav-item-dropdown>
      <b-nav-item class="user" @click="$router.push('/signIn')">
        <img
        class="d-block img-margin"
        height="14"
        src="/user.svg"
        alt="image"
        />
      </b-nav-item>
    </b-nav>
  </div>
</template>