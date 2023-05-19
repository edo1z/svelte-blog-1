<script lang="ts">
	import { Editor, rootCtx } from '@milkdown/core';
	import { commonmark } from '@milkdown/preset-commonmark';
	import { nord } from '@milkdown/theme-nord';

	const editor = Editor.make().config(nord).use(commonmark);

	console.log('status1', editor.status);

	const createEditor = (dom: any) => {
		editor
			.config((ctx) => {
				ctx.set(rootCtx, dom);
			})
			.create()
			.then(() => {
				console.log('status2', editor.status);
			});
	};
</script>

<div use:createEditor />
