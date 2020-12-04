<template>
    <section class="counter">
        <div class="">
            <h5>Contador</h5>
        </div>
        <div class="">
            <h1 class="counter-number">{{counter}}</h1>
            <button type="submit" @click="addCounter()" class="btn btn-primary">Count</button>
        </div>
    </section>
</template>

<script>
export default {
    name: "Counter",
    data() {
        return {
            counter: 0
        }
    },
    methods: {
        addCounter() {
            this.counter++
        }
    }
}
</script>

<style scoped>
.form-group {
    margin-bottom: 1rem;
}
.form-control {
    display: block;
    width: 100%;
    height: calc(1.5em + .75rem + 2px);
    padding: .375rem .75rem;
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.5;
    color: #495057;
    background-color: #fff;
    background-clip: padding-box;
    border: 1px solid #ced4da;
    border-radius: .25rem;
    transition: border-color .15s ease-in-out,box-shadow .15s ease-in-out;
}
.btn {
    cursor: pointer;
    display: inline-block;
    font-weight: 400;
    color: #212529;
    text-align: center;
    vertical-align: middle;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    background-color: transparent;
    border: 1px solid transparent;
    padding: .375rem .75rem;
    font-size: 1rem;
    line-height: 1.5;
    border-radius: .25rem;
    text-transform: uppercase;
    transition: color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;
}
.btn-primary {
    color: #fff;
    background-color: #6542f4;
    border-color: #6542f4;
}
.btn-primary.focus {
    color: #fff;
    background-color: #0069d9;
    border-color: #0062cc;
    box-shadow: 0 0 0 0.2rem rgba(38,143,255,.5);
}
.counter-number {
    font-size: 5rem;
}
</style>