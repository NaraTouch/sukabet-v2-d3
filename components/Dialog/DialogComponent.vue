<template>
	<div id="custom-style">
		<b-modal hide-footer ref="disc" title="Hello" ok-only ok-variant="light" size="lg" body-bg-variant="dark" header-bg-variant="dark" header-text-variant="light" body-text-variant="light" footer-bg-variant="dark" footer-text-variant="light" title-class="text-light">
			 <template #modal-title>
				<!-- Using <code>$bvModal</code> Methods -->
				<slot name="slot-title"></slot>
			</template>
			<div class="text-justify modal-text">
				<slot name="slot-body"></slot>
			</div>
		</b-modal>
	</div>
</template>

<script>
import slots from '~~/pages/slots.vue';
export default {
  components: { slots },
    methods: {
        showModal() {
            this.$refs['disc'].show()
        },
        hideModal() {
            this.$refs['disc'].hide()
        },
    },

    mounted() {
        console.log('Modal mounted.');
        if(localStorage.getItem('wasVisited') === null) this.showModal();
        localStorage.setItem('wasVisited', '1');
    }
}
</script>