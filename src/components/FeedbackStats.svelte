<script>
  import { feedbackStore } from "../stores";

  $: count = $feedbackStore.length;
  $: average =
    $feedbackStore.reduce((a, { rating }) => a + rating, 0) /
    $feedbackStore.length;
</script>

<div class="feedback-stat">
  <h4>{count} Reviews</h4>
  <h4>Rating Average: {average}</h4>
</div>

<style>
  .feedback-stat {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>
