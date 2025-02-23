<script lang="ts">
  import { Link } from 'svelte-routing';
</script>

<style>
  .blog-container {
    text-align: center;
    padding: 50px;
    max-width: 800px;
    margin: 0 auto;
  }

  .blog-header {
    font-size: 2.5rem;
    font-weight: bold;
    color: #fff;
    text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.7);
  }

  .blog-subtitle {
    font-size: 1.2rem;
    color: #ddd;
    margin-bottom: 20px;
  }

  .blog-background {
    background: url('https://i.pinimg.com/originals/09/35/7d/09357dc881925eb4859b7a03714a58be.jpg') center/cover no-repeat;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .button-group {
    margin-top: 20px;
  }

  .button {
    background: #ff6f61;
    color: white;
    border: none;
    padding: 12px 20px;
    margin: 10px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    transition: background 0.3s;
  }

  .button:hover {
    background: #e85a50;
  }
</style>

<!-- Hero Section -->
<div class="blog-background">
  <h1 class="blog-header">Welcome to My Personal Blog</h1>
</div>

<!-- Blog Content -->
<div class="blog-container">
  <h2 class="blog-subtitle">
    A space to share my thoughts, experiences, and creative projects.
  </h2>

  <p>
    Life is a journey, and every day brings new stories worth sharing. Whether it's tech, travel, photography, or personal reflections, you'll find it all here. Join me on this adventure!
  </p>

  <div class="button-group">
    <button class="button">
      <Link to="/posts">📖 Read My Blog</Link>
    </button>
    <button class="button">
      <Link to="/about">👤 About Me</Link>
    </button>
    <button class="button">
      <a href="https://github.com/Alejandralv9914" target="_blank" rel="noopener noreferrer">
        🌟 Follow me on GitHub
      </a>
    </button>
  </div>
</div>
