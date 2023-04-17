<template>
  <div>

      <div>Кол-вo лайков: <strong>{{ likes }}</strong> </div>
      <div>Кол-вo дизлайков: <strong>{{ dislikes }}</strong> </div>
      <div>
          <button v-on:click="addLike">Like</button>
          <button @click="addDisLike">Dislike</button>
      </div>
  </div>
</template>

<script>

export default {
    data() {
        return{
            likes: 0,
            dislikes: 0,
        }
    },
    methods: {
        addLike() {
            this.likes += 1;
        },
        addDisLike() {
            this.dislikes += 1;
        }
    }
}

</script>

<style>

</style>