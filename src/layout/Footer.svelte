<script lang="ts">
    const socialMedias = [
        {
            title: 'Risy Linkedin',
            name: 'Linkedin',
            url: 'https://www.linkedin.com/in/eren-m-952132229/',
        },
        {
            title: 'Risy Github',
            name: 'Github',
            url: 'https://github.com/therisy/'
        },
        {
            title: 'Discord Sunucularını Keşfet',
            name: 'Stalk.gg',
            url: 'https://stalk.gg/'
        }
    ];
</script>

<div class="h-20 w-full flex flex-col justify-center items-center">
    <span>Svelte Footer</span>


    <ul class="flex gap-4 mt-2">
        {#each socialMedias as sm}
            <li><a title={sm.title}  href="{sm.url}" target="_blank" class="hover:text-blue-400">{sm.name}</a></li>
        {/each}
    </ul>
</div>