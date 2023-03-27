<template>
  <div class="marquee-container">
    <div class="marquee-content">
      <p>{{ marqueeText }}</p>
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Marquee',
  data() {
    return {
      marqueeText: 'Jurassic Park'
    }
  }
}
</script>

<style>
.marquee-container {
  width: 100%;
  height: 50px;
  overflow: hidden;
  position: relative;
}

.marquee-content {
  width: 100%;
  height: 50px;
  position: absolute;
  animation: marquee 20s linear infinite;
}

.marquee-content p {
  display: inline-block;
  white-space: nowrap;
  font-size: 20px;
  color: white;
}

@keyframes marquee {
  0% { left: 100%; }
  100% { left: -100%; }
}
</style>
