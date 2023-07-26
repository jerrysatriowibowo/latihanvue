<template>
    <Navbar>
      <template #logo>
        <NavbarLogo image-url="./picture/helm5.jpg">HelmetID</NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Beranda</NavbarLink>
          <NavbarLink>Servis</NavbarLink>
          <NavbarLink>Tentang</NavbarLink>
          <NavbarLink>Kontak</NavbarLink>
        </NavbarCollapse>
      </template>
    </Navbar>
</template>
<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>