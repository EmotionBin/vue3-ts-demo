<template>
  <div class="container">
    <div class="forms-container">
      <div class="signin-signup">
        <h1>登录</h1>
        <h1>注册</h1>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { reactive, toRefs } from 'vue'
// interface dataProps{

// }
export default {
  name: 'LoginRegister',
  setup () {
    const data = reactive({

    })
    const refData = toRefs(data)
    return {
      ...refData
    }
  }
}
</script>

<style lang="scss">
.container {
  position: relative;
  width: 100%;
  background-color: #fff;
  min-height: 100vh;
  overflow: hidden;
}

.forms-container {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
}

.signin-signup {
  position: absolute;
  top: 50%;
  transform: translate(-50%, -50%);
  left: 75%;
  width: 44%;
  transition: 1s 0.7s ease-in-out;
  display: grid;
  grid-template-columns: 1fr;
  z-index: 5;
}
</style>
