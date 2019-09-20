<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https://www.moc.gov.tw/" target="_blank">
              Ministry Of Culture
            </a>
          </li>
          <li>
            <a href="https://clab.org.tw/" target="_blank">
              C-LAB
            </a>
          </li>
          <li>
            <a href="https://www.beehivedt.com/" target="_blank">
              Beehive Data Technology
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; Coopathon  {{ year }}. All Rights Reserved.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
