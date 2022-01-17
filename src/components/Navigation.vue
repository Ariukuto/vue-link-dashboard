<template>

    <div id="NavigationComponent">
        <div class="brandrow">
            <img :src="logo" class="brand" />
            <div class="brand-links">
                
            </div>
        </div>
        <div class="links"> 
            <div  v-for="link in sortedLinks" :key="link.title" class="link">
                {{link.title}}
            </div>  
        </div>

    </div>
      
</template>
<script>

    import {sortAlphabetical} from '../functions';

    export default {
        name: 'Navigation', 
        setup() {
            const {logo, links} = require("../mocks/NavigatonMock").data; 
            const sortedLinks = sortAlphabetical(links);
            return {
                logo,
                sortedLinks
            }
        }
    }

</script>
<style lang="css">
    #NavigationComponent {
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items:center;
    }
    .links {
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
    }
    .brand-links {
        display: flex;
    }
</style>

