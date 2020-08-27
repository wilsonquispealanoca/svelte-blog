<script>
  import Blog from "./blog/index.svelte";
  const siteTitle = "Wilson Quispe";
  export let segment;
</script>

<style>
  .headingMd {
    font-size: 1.2rem;
    line-height: 1.5;
  }

  .headingLg {
    font-size: 1.5rem;
    line-height: 1.4;
    margin: 1rem 0;
  }
</style>

<svelte:head>
  <title>{siteTitle}</title>
</svelte:head>

<section class="headingMd">
  <p>
    Hello, I’m
    <strong>Wil</strong>
    . I’m a software engineer, artist and a writer. You can contact me on{' '}
    <a href="https://twitter.com/soywill_quispe">Twitter</a>
    .
  </p>
  <p>
    (This is a sample website - you’ll be building a site like this in{' '}
    <a href="https://nextjs.org/learn">our Next.js tutorial</a>
    .)
  </p>
</section>
<section className="headingMd padding1px">
  <a
    rel="prefetch"
    aria-current={segment === 'blog' ? 'page' : undefined}
    href="blog">
    <h2 class="headingLg">Blog</h2>
  </a>
</section>
