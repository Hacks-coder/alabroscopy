<script>
	import Small from "../Texts/Small.svelte";

    const footer = [
        {href: "/home", child: "Home"},
        {href: "/home", child: "Services"},
        {href: "/home", child: "Contact"},
        {href: "/home", child: "Sign-up"}
    ]
</script>

<footer class="text-center mt-20 text-white  py-5  p-2">
    <div class="flex justify-between">
        <div>logo</div>
        <div class="space-x-3">
            {#each footer as {href, child}}
                <a {href} class="font-main">{child}</a>
            {/each}
        </div>
    </div>
    <hr class="mt-10 border-1 mb-2 border-purple">
    <Small text = "&copy Copyrights 2025. All Right Reserved"/>
</footer>