<script>
    export let icon;
    export let info;
    import {GithubSolid, LinkedinSolid, PhoneSolid, MailBoxSolid} from 'flowbite-svelte-icons';
    let color = "text-sky-500"
</script>
<span class="flex gap-x-2 items-center">
    {#if icon == "phone"}
        <PhoneSolid class={color}/>
    {:else if icon == "mail"}
        <MailBoxSolid class={color}/>
    {:else if icon == "github"}
        <GithubSolid class={color}/>
    {:else if icon == "linkedin"}
        <LinkedinSolid class={color}/>
    {/if}
    <p>{info}</p>
</span>
