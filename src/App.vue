<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <div>
        <h1>Sociologists on Mastodon</h1>
        <!-- Subtitle -->
        <p style="margin-top: 0px;">Follow all your favourite sociologists</p>
      </div>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/instructions">Instructions</RouterLink>
        <a href="https://github.com/nathanlesage/academics-on-mastodon" target="_blank">More lists from other disciplines</a>
      </nav>
    </div>
  </header>

  <RouterView />

  <!-- footer -->
  <hr/>
  <footer>
    Brought to you by
    <a href="https://social.tchncs.de/@perspektivbrocken" target="_blank">David Adler</a>,
    <a href="https://social.tchncs.de/@thhaase" target="_blank">Thomas Haase</a>
    &amp;
    <a href="https://scholar.social/@hendrikerz" target="_blank">Hendrik Erz</a>.
    If you want to contribute, please visit our
    <a href="https://github.com/trutzig89182/Mastodon-Sociologists" target="_blank">GitHub-Repository</a>.
  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
  border-bottom: 1px solid rgba(0, 0, 0, .8);
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  display: flex;
}

nav a {
  color: inherit;
}

nav a.router-link-exact-active {
  color: #1cb27e;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  text-decoration: none;
  padding: 0.5rem 1rem;
  border-left: 1px solid rgba(0, 0, 0, 0.4);
}

nav a:first-of-type {
  border: 0;
}

nav a:hover {
  background-color: rgba(0, 0, 0, .2);
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
  }
}
</style>
