
<template>
    <div class="withMargin"> 
        <button @click="hide"> {{ obj.hidden ? 'Показать' : 'Скрыть' }} </button>
        <p :class="obj">Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore voluptas suscipit soluta obcaecati doloremque nam eos culpa ullam exercitationem.</p>
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