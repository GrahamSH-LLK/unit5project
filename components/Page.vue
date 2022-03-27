<template>
  <div class="min-h-screen">
    <Nav class="mx-auto"/>
    <div class="flex flex-col justify-center">
      <Header>{{ title }}</Header>
      <Body>
        <slot />
      </Body>
    </div>
  </div>
</template>
<script>
export default {
  props: ["title"],
};
</script>
