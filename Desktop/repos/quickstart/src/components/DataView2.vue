<template>
    <div>
        <div>
            {{ selectedEvent }}
        </div>
    </div>
</template>

<script>
export default {
    name: "data-view2",
    computed: {
        selectedEvent: function() {
            return this.$store.state.selectdEvent;
        }
    }
}
</script>