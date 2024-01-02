<script>
  import FeedbackList from "./components/FeedbackList.svelte";
  import FeedbackStats from "./components/FeedbackStats.svelte";
  import FeedbackForm from "./components/FeedbackForm.svelte";
  //   let firstName = "Brad";
  //   let lastName = "Traversy";
  //   let color = "blue";
  //   let showText = false;
  //   let users = [
  //     {
  //       id: "1",
  //       name: "Eben",
  //     },
  // 	{
  //       id: "2",
  //       name: "Brist",
  //     },
  // 	{
  //       id: "3",
  //       name: "Donwing",
  //     },

  //   ];
  //   $: name = firstName + " " + lastName;

  //   const toggle = () => {
  //     color = color === "blue" ? "red" : "blue";
  //     showText = !showText;
  // 	users = [...users, {
  // 		id: "4",
  //       name: "Bob",
  // 	}]
  //   };

</script>

<main class="container">
  <FeedbackForm />
  <FeedbackStats/>
  <FeedbackList />
  <!-- {#if showText}
    <p>
      Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
      how to build Svelte apps.
    </p>
  {:else}
    <p>No Text</p>
  {/if}
  <button on:click={toggle} class="btn">Click</button>
  {#each users as user (user.id)}
    <h3>{user.id}: {user.name}</h3>
  {/each} -->
</main>
