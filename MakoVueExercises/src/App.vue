
<template>
	<p :class="obj">aLLO</p>
</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            obj: {
			red_color: true,
			font_big_size:  true,
		},
	}
},
    methods: 
    {


    computed: 
    {    
    }


    }
}

</script>

<style>


@import url('./styles/baton_styles.css');
@import url('./styles/page.css');
@import url('./styles/style.css');
</style>