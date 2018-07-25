// template只能暴露一个标签在外面
<template>
	<div>
		<home-header></home-header>
    <home-swiper></home-swiper>
    <home-icons></home-icons>
		<!-- <router-link to="/list" class="home">列表页</router-link> -->
	</div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
export default {
  name: 'Home',
  components: {
    HomeHeader: HomeHeader,
    HomeSwiper: HomeSwiper,
    HomeIcons: HomeIcons
  }
}
</script>

<style>

</style>
