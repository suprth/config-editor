<script>
    let fileinput;
    let a;

    const onFileSelected =(e)=>{
    let json = e.target.files[0];
            let reader = new FileReader();
            reader.readAsDataURL(json);
            reader.onload = e => {
                 console.log(e.target.result);
                 a = e.target.result;
            };
}
    
</script>

<img class="upload" src="https://static.thenounproject.com/png/625182-200.png" alt="" on:click={()=>{fileinput.click();}} />
<input style="display:none" type="file" accept=".json" on:change={(e)=>onFileSelected(e)} bind:this={fileinput} >

{#if a}
<p>{a}</p>
{/if}
<style>

</style>

