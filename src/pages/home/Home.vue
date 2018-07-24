// template只能暴露一个标签在外面
<template>
	<div>
		<home-header></home-header>
    <home-swiper></home-swiper>
		<!-- <router-link to="/list" class="home">列表页</router-link> -->
	</div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
export default {
  name: 'Home',
  components: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper
  }
}
</script>

<style>

</style>
