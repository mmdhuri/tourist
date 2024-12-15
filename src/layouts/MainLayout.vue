<template>
  <q-layout view="lHh Lpr lFf">
    <div class="home-header">
      <div class=" flex justify-between items-center container">
        <div>
          <router-link to="/" class="menu-item q-px-sm text-weight-medium">
            <img src="~src/assets/Site Images/logo.png" width="80">
          </router-link>
        </div>
        <div class="flex">
          <div class="menu">
            <router-link to="/" class="menu-item q-px-sm text-weight-medium">
              Home
            </router-link>
          </div>
          <div class="menu">
            <router-link to="/about-us" class="menu-item q-px-sm text-weight-medium">
              About Us
            </router-link>
          </div>
          <div class="menu">
            <router-link to="/contact-us" class="menu-item q-px-sm text-weight-medium">
              Contact Us
            </router-link>
          </div>
          <div class="menu">
            <router-link class="menu-item q-px-sm text-weight-medium">
              Destinations
            </router-link>
          </div>
        </div>
        <div></div>
      </div>
    </div>
    <q-page-container>
      <router-view />
    </q-page-container>

    <footer class="footer">
      <div class="container">
        <div class="row">
          <div class="footer-col">
            <h4>company</h4>
            <ul class="q-pl-sm">
              <li>
                <router-link to="/" class="menu-item text-weight-medium">
                  Home
                </router-link>
              </li>
              <li>
                <router-link to="/about-us" class="menu-item text-weight-medium">
                  About Us
                </router-link>
              </li>
              <li>
                <router-link to="/contact-us" class="menu-item text-weight-medium">
                  Contact Us
                </router-link>
              </li>
              <li>
                <router-link class="menu-item text-weight-medium">
                  Destinations
                </router-link>
              </li>
            </ul>
          </div>
          <div class="footer-col">
            <h4>follow us</h4>
            <div class="social-links">
              <a href="javascript:void(0)"><i class="fab fa-facebook-f"></i></a>
              <a href="javascript:void(0)"><i class="fab fa-twitter"></i></a>
              <a href="javascript:void(0)"><i class="fab fa-instagram"></i></a>
              <a href="javascript:void(0)"><i class="fab fa-linkedin-in"></i></a>
            </div>
          </div>
        </div>
        <hr>
        <div class="" align="center">
          <p class="q-mb-none text-white">{{ currentYear }} Designed & Developed by <a
              href="mailto:manishdhuri2000@gmail.com" class="text-white">Manish
              Dhuri</a> </p>
        </div>
      </div>
    </footer>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'

defineOptions({
  name: 'MainLayout'
})
const slide = ref(1);

const linksList = [
  {
    title: 'Docs',
    caption: 'quasar.dev',
    icon: 'school',
    link: 'https://quasar.dev'
  },
  {
    title: 'Github',
    caption: 'github.com/quasarframework',
    icon: 'code',
    link: 'https://github.com/quasarframework'
  },
  {
    title: 'Discord Chat Channel',
    caption: 'chat.quasar.dev',
    icon: 'chat',
    link: 'https://chat.quasar.dev'
  },
  {
    title: 'Forum',
    caption: 'forum.quasar.dev',
    icon: 'record_voice_over',
    link: 'https://forum.quasar.dev'
  },
  {
    title: 'Twitter',
    caption: '@quasarframework',
    icon: 'rss_feed',
    link: 'https://twitter.quasar.dev'
  },
  {
    title: 'Facebook',
    caption: '@QuasarFramework',
    icon: 'public',
    link: 'https://facebook.quasar.dev'
  },
  {
    title: 'Quasar Awesome',
    caption: 'Community Quasar projects',
    icon: 'favorite',
    link: 'https://awesome.quasar.dev'
  }
]

const currentYear = new Date().getFullYear() // Get the current year
const leftDrawerOpen = ref(false)

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value
}
</script>
