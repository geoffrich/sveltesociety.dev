<script>
  import { metatags } from "@roxi/routify";
  export let title,
    description = "";

  $: metatags.title = title;
  $: metatags.description = description;

  $: metatags["twitter:title"] = title;
  $: metatags["twitter:description"] = description;
</script>

<h1>{title}</h1>

<slot />
