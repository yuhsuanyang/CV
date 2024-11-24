<script>
    export let institute;
    export let location;
    export let position;
    export let duration;
</script>
<div class="flex justify-between my-2">
    <p class="font-bold">{institute}</p>
    <p>{location}</p>
</div>
<div class="flex italic justify-between ml-4"> <!-- my-2"-->
    <p>{position}</p>
    <p>{duration}</p>
</div>
<div class="ml-4">
    <slot/>
</div>

