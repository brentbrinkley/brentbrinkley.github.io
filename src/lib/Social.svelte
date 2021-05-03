<script>
  export let socLink
  export let title
  export let vector
</script>

<a class="link" href={socLink}>
  <svg
    class="h-6 fill-current text-gray-500 hover:text-yellow-400 transition duration-300"
    role="img"
    viewBox="0 0 24 24"
    xmlns="http://www.w3.org/2000/svg"
    ><title>{title}</title><path d={vector} /></svg
  >
</a>
