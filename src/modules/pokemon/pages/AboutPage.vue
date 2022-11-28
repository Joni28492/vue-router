<template>
    <h1>About Page</h1>
    <hr>
    <h2> {{name}} </h2>
    <button @click="onChangeName" >cambiar nombre</button>
</template>


<script>
export default {

    data(){
        return { 
            name: 'Joni',
        }
    },

    methods: {
        onChangeName(){
            // console.log('Se cambiara el nombre')
            this.name = "Jonathan"
            // console.log(this.name)
        }

    },

    //beforeCreate se carga antes que la data
    beforeCreate(){ console.log('beforeCreate') },
    //seria un buen punto para peticiones http
    created(){ 
        
        
        console.log('created') 
        
        
    },


    beforeMount(){ console.log('beforeMount') },
    mounted(){ console.log('mounted') },
    beforeUpdate(){ console.log('beforeUpdate') },
    updated(){ console.log('updated') },
    activated(){ console.log('activated') },
    deactivated(){ console.log('deactivated') },
    beforeUnmount(){ console.log('beforeUnmount') },
    unmounted(){ console.log('unmounted') },
    errorCaptured(){ console.log('errorCaptured') },
    renderTracked(){ console.log('renderTracked') },
    renderTriggered(){ console.log('renderTriggered') }
}
</script>