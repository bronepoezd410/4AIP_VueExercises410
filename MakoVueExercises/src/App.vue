
<template>
    <div class="withMargin"> 
        <p :class="{isActive: active, hasError: valid}"> text </p>
    </div>
</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
		active: false,
		valid: true,
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