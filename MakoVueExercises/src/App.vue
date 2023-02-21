
<template>
    <div class="withMargin"> 



        <input type="text" v-model="message" class="my-input">
        
        <p :style="{textTransform:'uppercase'}">{{ message }}</p>    

    </div>


    <div class="withMargin">
                
        <input type="number" v-model="number" class="my-input">

        <p :style="{textTransform:'uppercase'}">{{ number**2 }}</p>    

    </div>
</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
        message: 'азазазаз',
        number: 0
	}
},
    methods: 
    {}
}

</script>

<style>


@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');
</style>