<script>
  const name = "Wilson Quispe";
  export const siteTitle = "Sapper Sample Website";
  export let segment;
</script>

<style>
  .header {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .headerHomeImage {
    width: 8rem;
    height: 8rem;
  }

  .heading2Xl {
    font-size: 2.5rem;
    line-height: 1.2;
    font-weight: 800;
    letter-spacing: -0.05rem;
    margin: 1rem 0;
  }

  .borderCircle {
    border-radius: 9999px;
  }
</style>

<svelte:head>
  <title>Welcome</title>
  <meta
    name="description"
    content="Learn how to build a personal website using Sapper and Svelte.js" />
  <meta
    property="og:image"
    content={`https://og-image.now.sh/${encodeURI(siteTitle)}.png?theme=light&md=0&fontSize=75px&images=https%3A%2F%2Fassets.vercel.com%2Fimage%2Fupload%2Ffront%2Fassets%2Fdesign%2Fnextjs-black-logo.svg`} />
  <meta name="og:title" content={siteTitle} />
  <meta name="twitter:card" content="summary_large_image" />
</svelte:head>

<nav class="header">
  <a aria-current={segment === undefined ? 'page' : undefined} href=".">
    <img
      src="perfilWilson.jpg"
      class="headerHomeImage borderCircle"
      alt={name} />
  </a>
  <h1 class="heading2Xl">{name}</h1>
</nav>
