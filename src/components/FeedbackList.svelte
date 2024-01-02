<script>
  import { feedbackStore } from "../stores";
  // import {onMount, onDestroy} from 'svelte';
  import { fade, scale } from "svelte/transition";
  import FeedbackItem from "./FeedbackItem.svelte";
  //   export let feedBack = [];

  //  const unSubscribe = feedbackStore.subscribe((data) => feedBack = data)

  //   onMount(() => {
  //     console.log('mounted')
  //   })
  //   onDestroy(() => {
  //     unSubscribe()
  //   })
</script>

{#each $feedbackStore as fb (fb.id)}
  <div in:scale out:fade={{ duration: 500 }}>
    <FeedbackItem item={fb} />
  </div>
{/each}
