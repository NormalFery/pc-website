<!-- Copyright (c) 2023-2024 Ampflower
	 SPDX-License-Identifier: MIT
	 https://git.pridecraft.gay/website/blob/HEAD/LICENSE-BADGE -->
<script lang="ts">
	import BadgeRaw from '$lib/components/BadgeRaw.svelte';
	import type Badge from '$lib/types';
	export let badge: Badge;
	export let id = badge.id;
	export let rel = badge.rel;
	export let ext = badge.ext;
	export let link = badge.link;
	export let name = badge.name;
	export let head = badge.head;
	export let title = badge.title || `${head} ${name}`;
</script>

<BadgeRaw {rel} {id} {link} {name} {title} {head} {ext} />
