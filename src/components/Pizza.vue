<template>
    <div>
        <h2> Pizza Name: {{pizzaName}}</h2>
        <p>Price: {{pizzaPrice}}</p>
        <p>Size: {{pizzaSize}}</p>
                <div>
            <slot name='n1'>
            </slot>
            <slot>
            </slot>
        </div>
    </div>
</template>

<script>
export default {
    props: ['pizzaName','pizzaPrice', 'pizzaSize'],    
}
</script>
