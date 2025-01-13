<script lang="ts">
    let { img, onclick } = $props();
</script>
<div class="avatar">
	<div class="w-24 rounded-full ring ring-primary ring-offset-2 ring-offset-base-100" onclick={onclick}>
		<img src={img} />
	</div>
</div>
