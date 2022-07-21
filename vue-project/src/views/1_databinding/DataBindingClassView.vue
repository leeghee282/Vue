<template>
  <div>
    <div :class="{'text-red': true}">클래스 바인딩</div>
    <div :class="{'text-red': false}">클래스 바인딩</div>
    <div :class="{'text-red': true, active: true}">클래스 바인딩</div>
    <div :class="{'text-red': hasError, active: isActive}">클래스 바인딩</div>
    <br>
    <div :class="class2">클래스 바인딩2</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: false,
      hasError: false,
      class2: ['active', 'hasError']
    }
  }
}
</script>

<style>
.active {
  background-color: greenyellow;
  font-weight: bold;
}

.text-red {
  color: red;
}
</style>
