<script>
	import { NAME } from '../constants';
</script>

<footer>
	<div class="top-row">
		<img src="favicon.png" height="24" width="24" alt="logo" />
		<div style="width: 12px" />
		<p>{NAME}</p>
	</div>
    <div class="top-row">
		<p>Copyright, 2023</p>
	</div>
</footer>

<style>
	.top-row {
		display: flex;
		align-items: center;
	}
	footer {
		display: flex;
        margin-top: 5rem;
        justify-content: space-between;
	}
</style>
