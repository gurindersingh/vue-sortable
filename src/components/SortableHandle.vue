<script>
    export default {
        name: "vue-sortable-handle",

        render() {
            return this.$slots.default[0]
        },
        inject: ['handleClass'],
        mounted() {
            this.$el.classList.add(this.handleClass)
        }
    }
</script>