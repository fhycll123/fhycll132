// template只能暴露一个标签在外面
<template>
	<div>
		<home-header></home-header>
		<!-- <router-link to="/list" class="home">列表页</router-link> -->
	</div>
</template>

<script>
import HomeHeader from './components/Header'
export default {
  name: 'Home',
  components: {
    HomeHeader: HomeHeader
  }
}
</script>

<style>

</style>
