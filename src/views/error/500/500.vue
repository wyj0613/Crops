<template>
  <v-app class="exception">
    <v-container fluid fill-height>
      <v-layout align-center justify-center row>
        <div class="mr-3 hidden-sm-and-down">
          <img :src="require('@/assets/images/error/500.svg')" alt />
        </div>
        <div class="text-md-center">
          <h1>500</h1>
          <h2 class="my-3 headline">啊咧，服务器飞走了!</h2>
          <div>
            <v-btn color="primary" large class="light headline" @click="goHome">主&nbsp;&nbsp;页</v-btn>
          </div>
        </div>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
export default {
  methods: {
    goHome () {
      this.$router.push({ path: '/' })
    }
  }
}
</script>
<style scoped lang="css">
h1 {
  font-size: 150px;
  line-height: 150px;
  font-weight: 700;
  color: #252932;
  text-shadow: rgba(61, 61, 61, 0.3) 1px 1px, rgba(61, 61, 61, 0.2) 2px 2px, rgba(61, 61, 61, 0.3) 3px 3px;
}
</style>
