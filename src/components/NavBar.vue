<template lang="pug">
.navbar
  router-link.title(to="/") My vue3 study
  nav.list
    MyButton.btn(@click="$router.push('/posts')") Страница с постами
    MyButton.btn(@click="$router.push('/store')") Страница с постами (store)
    MyButton.btn(@click="$router.push('/composition')") Страница с постами (Composition api)

    MyButton.btn(@click="$router.push('/')") О сайте
</template>
<script>
export default {
  components: {},
};
</script>
<style lang="scss">
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: teal;
  padding: 10px 20px;

  .title {
    color: white;
    font-size: 24px;
    text-decoration: none;
  }
  .list {
    display: flex;
    justify-content: flex-end;
  }

  .btn {
    border-color: white;
    color: white;
    margin-left: 20px;

    &:hover {
      border-color: white;
    }
  }
}
</style>