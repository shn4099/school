<template>
	<div class="Outnews">
		<ul class="ulnews">
			<li class="linews">
				<a href='#' target="_blank">百度新新新新新新新新新新新新新新新新新新新新新新新新闻</a>
			</li>
			<li class="linews" v-for=' content in contents' @clicknews='opennews()'>
				<span href='' target="_blank">{{content}}</span>
			</li>
		</ul>
	</div>
</template>

<script>
	export default {
		data(){
			return{
				contents:{},
			}
		},
		 created(){
    		this.getNews()
  		},
		methods:{
			opennews(){

			},
			getNews(){

			}
		}
	}
</script>

<style>
	.Outnews{
		width: 98%;
		min-height: 400px;
		background-color: gray;
		margin: 0 auto;
		margin-top:20px;
		margin-bottom: 20px; 
		border-radius: 10px;
	}
	.ulnews{
		margin: 0;
		padding: 0;
	}
	.linews{
		list-style: none;
		padding: 5px;		
		cursor: pointer;
		padding-left: 10px;
		min-height: 30px;
		border-bottom: 1px solid lightgrey;
	}
	.linews a,span{
		line-height: 30px;
		color: black;
		text-decoration: none;
		overflow:hidden;
 		word-break: break-all;
 		display: -webkit-box;
  			-webkit-line-clamp: 1; /*限制在一个块元素显示的文本的行数*/
  			-webkit-box-orient: vertical;
  		text-overflow:ellipsis;
	}
</style>
