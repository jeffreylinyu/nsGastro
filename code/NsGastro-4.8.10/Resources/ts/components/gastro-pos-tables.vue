<template>
    <div class="w-95vw h-95vh md:w-4/5-screen md:h-4/5-screen bg-white shadow-lg ">
        <div class="header border-b border-gray-200 p-2 flex justify-between items-center">
            <h3 class="font-bold">{{ __m( 'Table Management', 'NsGastro' ) }}</h3>
            <div>
                <ns-close-button @click="closePopup()"></ns-close-button>
            </div>
        </div>
        
    </div>
</template>
<script>
export default {
    name : "gastro-pos-tables",
    mounted() {
        this.popupCloser();
    },
    methods: {
        __m,
        popupCloser,
        popupResolver,
        closePopup() {
            this.popupResolver( false );
        }
    }
}
</script>