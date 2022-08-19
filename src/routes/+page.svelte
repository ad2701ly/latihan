<script>
    import { draw,slide } from "svelte/transition";
    import { quintOut } from "svelte/easing";

    let nomer=1+2
    let tampil=true
</script>
<layouts>
    <h2>Login</h2>
    <kotak> 
        <span>{nomer}</span>
        <span>{typeof nomer}</span>
    </kotak>
</layouts>

{#if tampil}
<backdrop on:click={()=>tampil=!tampil} transition:slide={{delay:2000}}>
    <svg viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
        {#if tampil}
            <path transition:draw="{{duration: 1500, easing: quintOut}}"
                        d="M 4 8 L 10 1 L 13 0 L 12 3 L 5 9 C 6 10 6 11 7 10 C 7 11 8 12 7 12 A 1.42 1.42 0 0 1 6 13 A 5 5 0 0 0 4 10 Q 3.5 9.9 3.5 10.5 T 2 11.8 T 1.2 11 T 2.5 9.5 T 3 9 A 5 5 90 0 0 0 7 A 1.42 1.42 0 0 1 1 6 C 1 5 2 6 3 6 C 2 7 3 7 4 8 M 10 1 L 10 3 L 12 3 L 10.2 2.8 L 10 1"
                        fill="none"
                        stroke="cornflowerblue"
                        stroke-width="0.1px"
                        />
        {/if}
    </svg>
</backdrop>
{/if}

<style>
    h2{
        text-align: center;
    }
    layouts{
        position: relative;
        display:grid;
        width: 100%;
        height: 100vh;
        background-color: rgba(0, 255, 85, 0.392);
       
    }
    kotak{
        display: block;
        background-color: white;
        margin: 0 2rem;
       padding: 2rem;
       border: 2px blue solid;
    }
    backdrop{
        width: 100vw;
        top: 0;
        left: 0;
        height: 100vh;
        position: fixed;
        z-index: 1;
        background-color: white;
    }
</style>