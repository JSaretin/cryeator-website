<script lang='ts'>
    export let advantage: {title:string;content: string}
</script>

<div>
    <h3 class="font-semibold text-lg text-gray-900">{advantage.title}</h3>
    <p class="text-slate-500 mt-2 leading-relaxed">
        {advantage.content}
    </p>
</div>