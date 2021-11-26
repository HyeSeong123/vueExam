<template>
	<TitleBar>홈 메인 페이지</TitleBar>

	<section class="article-write-form-box">
		<div class="container mx-auto">
			<form action="">
				<FormRow title="제목">
					<input class="form-row-input" type="text" placeholder="제목을 입력해주세요.">
				</FormRow>
				<FormRow title="내용">
					<textarea class="form-row-input" type="text" placeholder="제목을 입력해주세요."></textarea>
				</FormRow>
				<FormRow title="작성">
					<input type="button" value="작성" />
 				</FormRow>
			</form>
		</div>
	</section>
</template>

<script setup lang="ts">
	
</script>

<style>

</style>