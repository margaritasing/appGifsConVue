<template>
  <div class="footer">
      <footer class="text-center bg-dark text-white py-3 bg-gradient">
          <h2>&copy; {{ year }} - Libia M Freites M</h2>
      </footer>
  </div>
</template>

<script>
export default {
    data: () => ({
        year: new Date().getFullYear(),
    }),
};
</script>

<style>
.footer{
    position: fixed;
    bottom: 0;
    width: 100%;
}
</style>