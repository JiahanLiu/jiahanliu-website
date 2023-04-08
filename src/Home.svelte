<!-- Home.svelte -->
<script>
  // Import any data or functions needed for the page here
  const articles = [
    {
      title: "First article",
      date: "April 10, 2023",
      content: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    },
    {
      title: "Second article",
      date: "April 9, 2023",
      content: "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.",
    },
    {
      title: "Third article",
      date: "April 8, 2023",
      content: "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident.",
    },
  ];
</script>

<div class="articles">
  {#each articles as article}
    <div class="article">
      <h2>{article.title}</h2>
      <p>{article.date}</p>
      <p>{article.content}</p>
    </div>
  {/each}
</div>

<style>
  .articles {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 2rem;
  }

  .article {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 2rem;
    width: 80%;
    border: 1px solid #ccc;
    padding: 1rem;
    border-radius: 5px;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
  }

  h2 {
    margin-top: 0;
    font-size: 1.5rem;
  }

  p {
    margin-bottom: 0;
    text-align: center;
  }
</style>
