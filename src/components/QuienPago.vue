<template>
    <div class="container mt-3">
        <div class="row">
            <div class="col">
                <h3 class="text-center">Quién Pagó?</h3>
            </div>
        </div>
        <div class="row">
            <div class="col">
                <ul class="list-group">
                    <li v-for="(persona, index) in quienesPagaron" v-bind:key="index" class="list-group-item">
                        <div class="row">
                            <div class="col-6"> {{ persona.name }} </div>
                            <div class="col-4"> {{ persona.type }} </div>
                            <div class="col-2 text-right"> {{ persona.total }} </div>
                        </div>
                    </li>
                </ul>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'quien-pago',
    props: ['quienesPagaron']
}
</script>

<style scoped>
    .container{
        background-color: transparent;
    }
    .list-group-item{
        background-color: #192a56;
        border-color: #273c75;
        border-width: 2px;
    }
    .list-group-item:first-child {
        border-top-left-radius: .5rem;
        border-top-right-radius: .5rem;
    }
    .list-group-item:last-child {
        border-bottom-left-radius: .5rem;
        border-bottom-right-radius: .5rem;
    }
</style>
