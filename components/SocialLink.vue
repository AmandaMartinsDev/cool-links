<template>
  <a :href="socialLink" class="social-link" target="_blank" alt="altText">
    <i :class="fontAwesome"></i>
  </a>
</template>

<script>
export default {
  name: "SocialLink",
  props: {
    socialLink: String,
    altText: String,
    fontAwesome: String,
  },
};
</script>
<style scoped>
a {
  transition: all 0.7s ease;
  color: var(--light-blue);
  font-family: "Montserrat", sans-serif;
  text-transform: uppercase;
  text-align: center;
  line-height: 1;
  font-size: 25px;
  background-color: transparent;
  outline: none;
  border-radius: 11px;
  background-color: var(--blue);
}
a:hover {
  color: var(--blue);
  background-color: var(--white);
}
a:hover i {
  color: var(--blue);
}
i {
  color: var(--white);
}
</style>
