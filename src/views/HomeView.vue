<script setup lang="ts">
</script>

<template>
  <main>
    <!-- Description paragraph -->
    <p>
        You want to get in touch with sociologists from around the world on
        <a
          href="https://en.wikipedia.org/wiki/Mastodon_(software)"
          target="_blank"
          >Mastodon</a
        >? This page lists accounts from sociologists and sociological
        institutions and offers an easy method to follow multiple accounts at
        once. Just decide if you want to follow all or only some of the accounts
        listed below. You are provided with a .csv-file, which you can upload in
        Mastodon in order to follow all accounts included.
        <a href="instructions.pdf" target="_blank">Here</a> you can find an
        short instruction, on how to do this.
      </p>

    <!-- Buttons - do not change -->
      <div>
        <button type="button" id="select-all-users">Select all</button>
        <button type="button" id="select-none-users">Select none</button>
        <button type="button" id="get-complete-csv">Get CSV for entire list</button>
      </div>

      <!-- checkbox section - do not change -->
      <form id="main-form" method="get" action="#">
        <fieldset>
          <legend>
            Accounts by handle, name, and profile link (most recent first)
          </legend>
          <div id="user-list"></div>
          <button type="button" id="generate-csv">Get CSV for selected accounts</button>
        </fieldset>
      </form>

      <!-- further information and contact-->
      <p>
        Full names are only included if they are shown in the profile or on
        explicit demand. You want to get on the list? Or you don’t want to be on
        it anymore? Please contact me
        <a href="mailto:david.adler@uni-oldenburg.de?subject=SoM%3A%20include%20me%21" target="_blank">via email</a>
        (preferred) or under
        <a href="https://social.tchncs.de/@perspektivbrocken" target="_blank">@perspektivbrocken@social.tchncs.de</a>.
      </p>

      <p>
        You are interested in sociological content on mastodon, but you don’t
        want to be added to the list? Then you could consider follwing the group
        <a href="https://a.gup.pe/u/sociology" target="_blank">@sociology@a.gup.pe</a>.
      </p>
  </main>
</template>
