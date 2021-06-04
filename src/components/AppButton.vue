<template>
    <a href="btnLink"><span class="rounded-md bg-red-500 text-sm py-2 px-4 text-white uppercase tracking-wide hover:bg-red-700"> {{ buttonValue }} </span></a>
</template>

<script>
export default {
    props: ['buttonValue']
}
</script>