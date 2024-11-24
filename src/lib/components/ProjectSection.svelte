<script>
    export let projectName;
    export let duration;
</script>
<div class="flex justify-between my-2">
    <p class="font-bold">{projectName}</p>
    <p ckass="italic ">{duration}</p>
</div>
<div class="ml-4">
    <slot/>
</div>

