<script>
	import Upload from './components/Upload.svelte'
</script>

<div class="main-container">
	<h1 class="app-title">CONFIG EDITOR</h1>
	<div class="upload-option-container">
		<Upload/>
	</div>
</div>

<style> 

	.main-container {
		background-color: #333;
	}
	.upload-option-container {
		width: 100%;
		height: 90vh;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.app-title {
		text-align: center;
		color: #f2f2f2;
	}
</style>