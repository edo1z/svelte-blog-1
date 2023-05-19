<script lang="ts">
	import { Editor, rootCtx } from '@milkdown/core';
	import { commonmark } from '@milkdown/preset-commonmark';
	import { nord } from '@milkdown/theme-nord';

	// components
	import TextEditor from '$lib/components/TextEditor/TextEditor.svelte';
	import WysiwygEditor from '$lib/components/WysiwygEditor/WysiwygEditor.svelte';
</script>

<div class="editor_container">
	<div>
		<TextEditor />
	</div>
	<div>
		<WysiwygEditor />
	</div>
</div>

<style>
	.editor_container {
		width: 100%;
		display: flex;
	}
	.editor_container div {
		width: 50%;
	}
</style>
