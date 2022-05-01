<template>
  <div :class="{ 'theme-helper': true, 'theme-helper-opened': opened }">
    <section class="widget theme-helper-content">
      <header class="theme-helper-header d-flex p-0">
        <div class="theme-helper-toggler" @click="toggle">
          <div class="theme-helper-spinner text-white">
            <i class="la la-cog"></i>
            <i class="la la-cog"></i>
          </div>
        </div>
        <h6>Configuration</h6>
      </header>
    </section>
  </div>
</template>

<script>
export default {
  name: "Helper",
  data() {
    return {
      opened: false,
    };
  },
  methods: {
    toggle() {
      this.opened = !this.opened;
    },
  },
};
</script>

<style src="./Helper.scss" lang="scss" scoped />
