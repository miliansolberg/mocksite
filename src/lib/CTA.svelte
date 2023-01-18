<script>
    function handleClick() {
        document.querySelector('button').style.backgroundColor='red';
        document.querySelector('button').innerHTML='Starting now...';
        document.querySelector('button').location.href='/';
   }
</script>

<button on:click={handleClick}>
Get Started
</button>

<style>
button {
    height: 6vh;
    width: 25vh;
    border-radius: 30px;
    background-color: rgb(195, 45, 45);
    border: 1px solid white;
    font-weight: 600;
    text-transform: capitalize;
}
</style>