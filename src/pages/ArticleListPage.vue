<template>
	<TitleBar>게시물 리스트</TitleBar>
	<section class="article-write-form-box">
		<div class="container mx-auto">
			<form v-on:submit.prevent="checkAndWrite">
				<FormRow title="제목">
					<input ref="newArticleTitleElRef" class="form-row-input" type="text" placeholder="제목을 입력해주세요.">
				</FormRow>
				<FormRow title="내용">
					<textarea ref="newArticleBodyElRef" class="form-row-input" type="text" placeholder="제목을 입력해주세요."></textarea>
				</FormRow>
				<FormRow title="작성">
					<div class="btns">
						<input type="button" class="btn_primary" value="작성" />
						<input type="submit" class="btn-secondary" value="작성" />
					</div>
 				</FormRow>
			</form>
		</div>
	</section>
</template>

<script lang="ts">
	import { defineComponent, ref } from 'vue'

	export default defineComponent({
		name : 'ArticleListPage',
		setup() {
			const newArticleTitleElRef =  ref<HTMLInputElement>();
			const newArticleBodyElRef =  ref<HTMLInputElement>();

			function checkAndWrite() {
				if ( newArticleTitleElRef.value == null ) {
					return;
				}

				newArticleTitleElRef.value.value = newArticleTitleElRef.value.value.trim();

				if ( newArticleTitleElRef.value.value.length == 0 ){

				}
			}

			return {
				checkAndWrite,
				newArticleTitleElRef,
				newArticleBodyElRef
			}
		}
	})
</script>

<style>

</style>