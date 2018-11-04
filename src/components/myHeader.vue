<template>
    <div id='header'>myHeader</div>
</template>

<script>
const header_height = 60

document.addEventListener("DOMContentLoaded", function(){
    const css_header = document.getElementById('header');
    css_header.style.height = header_height + 'px';
});

export default {
    name: 'myHeader',
    data: function(){
        return {
            header_height: header_height
        }
    }
}
</script>

<style>
    #header{
        background: #00ff00;
        width: 100%;
        position: fixed;
        top: 0;
        left: 0;
    }
</style>
