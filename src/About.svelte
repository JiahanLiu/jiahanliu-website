<!-- About/About.svelte -->

<script>
  const linkedinUrl = "https://www.linkedin.com/in/jiahan-jim-liu/";
  const githubUrl = "https://github.com/JiahanLiu";
  const twitterUrl = "https://twitter.com/jiahanjimliu";
</script>

<div class="container">
  <h1>About</h1>
  <img src="/ProfilePicture.jpeg" alt="Profile Picture" class="profile-picture" />
  <p>
    Learning about programming, technology, math, markets and health. 
    Learn by doing. 
    Picking methods that produce fast but executing at normal speeds. 
    Being a great person and identifying great individuals to work and have fun with.
  </p>
  <p>Connect with me on:</p>
  <ul class="social-links">
    <li>
      <a href="{linkedinUrl}" target="_blank" rel="noopener noreferrer">
        <i class="fab fa-linkedin"></i> LinkedIn
      </a>
    </li>
    <li>
      <a href="{githubUrl}" target="_blank" rel="noopener noreferrer">
        <i class="fab fa-github"></i> GitHub
      </a>
    </li>
    <li>
      <a href="{twitterUrl}" target="_blank" rel="noopener noreferrer">
        <i class="fab fa-twitter"></i> Twitter
      </a>
    </li>
  </ul>
</div>

<style>
  :root {
    --main-color: #0077b5;
    --hover-color: #005582;
  }

  .container {
    font-family: 'Roboto', sans-serif;
    max-width: 800px;
    margin: 0 auto;
    text-align: center;
  }
  h1 {
    font-size: 2em;
    margin-bottom: 0.5em;
    color: #000; /* Changed color to black */
  }
  .profile-picture {
    max-width: 200px;
    height: auto;
    border-radius: 50%;
    margin-bottom: 1em;
    display: block;
    margin-left: auto;
    margin-right: auto;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }
  p {
    line-height: 1.6;
  }
  ul.social-links {
    list-style-type: none;
    padding: 0;
  }
  ul.social-links li {
    display: inline;
    margin: 0 1em;
  }
  a {
    color: var(--main-color);
    text-decoration: none;
    transition: color 0.3s ease;
  }
  a:hover {
    color: var(--hover-color);
  }
  i {
    margin-right: 4px;
  }
</style>
