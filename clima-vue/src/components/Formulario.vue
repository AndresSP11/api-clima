<script setup>
const paises = [
    { codigo: 'US', nombre: 'Estados Unidos' },
    { codigo: 'MX', nombre: 'México' },
    { codigo: 'AR', nombre: 'Argentina' },
    { codigo: 'CO', nombre: 'Colombia' },
    { codigo: 'CR', nombre: 'Costa Rica' },
    { codigo: 'ES', nombre: 'España' },
    { codigo: 'PE', nombre: 'Perú' }
]
</script>

<template>
    <form
    class="formulario"
    >
        <div class="campo">
            <label for="">Ciudad</label>
            <input type="text"
            id="ciudad"
            placeholder="Ciudad">
        </div>
        <div class="campo">
            <label for="pais">Pais</label>
            <select name="" id="pais">
                <option value="">--Seleccione--</option>
                <option v-for="pais in paises" :value="pais.codigo">{{ pais.nombre }}</option>
            </select>
        </div>
        <input type="submit" value="Consultar Clima">
    </form>

</template>

<style scoped>
.campo select option{color: black;}

</style>