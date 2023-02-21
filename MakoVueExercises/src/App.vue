
<template>
    <div class="withMargin"> 













        <p :style="{color: 'green', backgroundColor: 'yellow'}"> Lorem ipsum, dolor sit amet consectetur adipisicing elit. Harum, possimus! </p>

        <p :style="{fontStyle:'italic'}"> <b>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor, beatae odit repellat eligendi fugit excepturi est? Sequi dicta voluptatum blanditiis molestias distinctio fugiat, repellat maiores facere, et quos doloremque reiciendis.</b> </p>
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