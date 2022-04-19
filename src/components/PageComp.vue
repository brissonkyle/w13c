<template>
    <div>
        <h1>Choose a Song!!</h1>
        <div id="gridContainer">
        <SongComp/>
        <PlaylistComp/>
        </div>
    </div>
</template>

<script>
import PlaylistComp from './PlaylistComp.vue'
import SongComp from './SongComp.vue'
    export default {
        components: { SongComp, PlaylistComp },
        name : 'PageComp',
        songNames: {
            songName : String,
            artistName : String
        },
    }
</script>

<style lang="scss" scoped>
#gridContainer {display: grid;
    grid-template-columns: 1fr 1fr;
}
</style>