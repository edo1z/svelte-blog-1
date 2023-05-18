<script lang="ts">
	import { Editor, rootCtx } from '@milkdown/core';
	import { commonmark } from '@milkdown/preset-commonmark';
	import { nord } from '@milkdown/theme-nord';

	const editor = (dom: any) => {
		Editor.make()
			.config((ctx) => {
				ctx.set(rootCtx, dom);
			})
			.config(nord)
			.use(commonmark)
			.create();
	};
</script>

<div use:editor />
