<template>
    <div id="app" data-v-app>
        <h1 id:="elementId" :class="elementClass">Heading</h1>
    </div>
</template>

<script>
let elementId = 'heading';
let elementClass = 'heading';
</script>

<style>
.heading {
  font-size: 24px;
  color: blue;
}
</style>
