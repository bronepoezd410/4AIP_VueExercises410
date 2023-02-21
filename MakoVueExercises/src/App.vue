
<template>
    <div class="withMargin"> 
        <p :class="{active: false, valid: true}">Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore voluptas suscipit soluta obcaecati doloremque nam eos culpa ullam exercitationem.</p>
    </div>
</template>




<script>
import { normalizeProps } from 'vue';

export default {
    data() {
        return {
            obj: {
			hidden: false,
		},
	}
},
    methods: 
    {
        hide: function(){
            this.obj.hidden = !this.obj.hidden;
        },


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