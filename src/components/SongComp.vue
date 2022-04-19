<template>
    <div>
            <h1>Song list</h1>
            <h3>Click a song to SAVE it !!</h3>
        <ul>
            <li
            :key="song.songName"
            v-for="song in songNames"
            :v-bind="song">
            <h2>{{song.artistName}}<button :class="select">Add Song</button></h2>
            <h3>{{song.songName}}</h3>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name : 'SongComp',
        data() {
            return {
                selected : false,
                methods: {
                    select() {
                        this.$emit('songClick')
                        this.selected = true;
                    }
                },
                songNames: [ 
                {
                    songName : 'Frozen Remix',
                    artistName : 'Sickick'
                },
                {
                    songName : 'Blacks Ops 2 Theme Song',
                    artistName : 'COD'
                },
                {
                    songName : 'Higher',
                    artistName : 'Bingx'
                },
                {
                    songName : 'Anilyst',
                    artistName : 'Sickick'
                },
                {
                    songName : 'Catch Up',
                    artistName : 'Anilyst'
                },
                {
                    songName : 'Energy',
                    artistName : 'Ryan Oakes'
                },
                {
                    songName : 'Just Lose It',
                    artistName : 'Eminem'
                },
                {
                    songName : 'Superman',
                    artistName : 'Eminem'
                },
                {
                    songName : 'No love',
                    artistName : 'Eminem'
                },
                {
                    songName : 'Daddys Lambo',
                    artistName : 'Yelawolf '
                },
                {
                    songName : 'Bingx',
                    artistName : 'I Know'
                },
                {
                    songName : 'Diamonds',
                    artistName : 'Rhianna'
                },
                {
                    songName : 'Everybody',
                    artistName : 'Stabilo'
                },
                {
                    songName : 'Whiskey Lullaby',
                    artistName : 'Brad Paisley'
                },
                {
                    songName : 'Eminem',
                    artistName : 'Mockingbird'
                },
                ],
                
            }
        },
        
    }
</script>

<style lang="scss" scoped>
    
</style>