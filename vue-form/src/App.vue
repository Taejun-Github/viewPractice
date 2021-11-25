<template>
  <div>
    <form v-on:submit.prevent="submitForm">
      <div>
        <label for="username">id: </label>
        <input id="username" type="text" v-model="username">
      </div>
      <div>
        <label for="password">password: </label>
        <input id="password" type="password" v-model="password">
      </div>
      <button type="submit">제출 버튼</button>
      <button type="reset">취소</button>
    </form>
  </div>
</template>

<script>



export default {
  data: function() {
    return {
      username: '',
      password: '',
    }
  },
  methods: {
    submitForm: function() {
      // event.preventDefault();
      console.log(this.username, this.password);
      // axois.post();
    }
  }
}
</script>

<style>

</style>