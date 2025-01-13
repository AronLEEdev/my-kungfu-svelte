<script lang="ts">
    import logo from '$lib/assets/LEE-LOGO.png';
    import Badge from './Badge.svelte';
	let { title } = $props();
</script>

<div class="navbar bg-base-100">
	<div class="flex-none">
		<div class="flex-1 flex justify-end">
            <img class="w-24 rounded-full" alt="myLogo" src={logo} />
        </div>
	</div>
	<div class="flex-1">
		<a class="btn btn-ghost text-xl">{ title }</a>
        <Badge content="powered by svelte" />
	</div>
	<div class="flex-none">
		<button class="btn btn-square btn-ghost">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				class="inline-block h-5 w-5 stroke-current"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z"
				></path>
			</svg>
		</button>
	</div>
</div>
