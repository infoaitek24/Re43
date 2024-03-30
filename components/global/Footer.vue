<template>
  <footer :class="$style.footer">
    <p>&copy; {{ new Date().getFullYear() }}  <a target="_blank" href="https://jason.codes/cookie-policy" rel="noopener">All rights reserved Momuflix Media</a></p>
    <p> <a target="_blank" href="https://www.themoviedb.org/" rel="noopener"></a></p>
  </footer>
</template>

<style lang="scss" module>
@import '~/assets/css/utilities/_variables.scss';

.footer {
  padding: 2rem 1.5rem 6.5rem;
  color: $text-color-grey;

  @media (min-width: $breakpoint-small) {
    padding-right: 4rem;
    padding-left: 4rem;
  }

  @media (min-width: $breakpoint-large) {
    padding: 2rem 5rem;
  }

  p {
    margin: 0.3rem 0;
    font-size: 1.4rem;
  }

  a {
    color: $text-color-grey;
    text-decoration: underline;
  }
}
</style>

