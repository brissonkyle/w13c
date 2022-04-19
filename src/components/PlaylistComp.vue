<template>
    <div>
        <h1>Playlist Selected</h1>
        <h3>Click a song to REMOVE it !!</h3>
        <div>
            
        </div>
    </div>
</template>

<script>

    export default {
        name : 'PlaylistComp',
        
    }
</script>

<style lang="scss" scoped>
button {
    display: none;
}
    ul{
        list-style-type: none;
        li{
            color: rgb(28, 28, 147);
            border-bottom: solid 2px crimson;
            margin: 10px;
        }
    }
</style>