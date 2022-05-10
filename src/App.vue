<template>
    <div>
        <div>
            One-way data binding <br>
            Two-way data binding <br>
            v-model -> formulários
        </div>

        <br><br>

        <div>
            <label>Nome</label> <br>
            <input
                v-model="name"
                type="text"
            > <br>
            {{ name }}
        </div>

        <br><br>

        <div>
            <label>Sports</label> <br>
            <select v-model="sports">
                <option value="">Escolha</option>
                <option value="futebol">Futebol</option>
                <option value="skate">Skate</option>
                <option value="Tenis">Tenis</option>
            </select> <br>
            {{ sports }}
        </div>

        <br><br>

        <div>
            <label>Newsletter</label> <br>
            <input
                v-model="newsletter"
                type="radio"
                value="Sim"
            > Sim

            <input
                v-model="newsletter"
                type="radio"
                value="Não"
            > Não <br>
            {{ newsletter }}
        </div>

        <br><br>

        <div>
            <label>Contrato</label> <br>
            <input
                v-model="contract"
                type="checkbox"
            > Aceita nosso termos... <br>

              {{ contract }}
        </div>

        <br><br>

        <div>
            <label>Cores que você mais gosta</label> <br>
            <input
                v-model="colors"
                type="checkbox"
                value="Azul"
            > Azul

            <input
                v-model="colors"
                type="checkbox"
                value="Amarelo"
            > Amarelo <br>
              {{ colors }}
        </div>
    </div>
</template>

<script>
export default {
    name: 'App',
    data() {
        return {
            name: 'jon snow',
            sports: 'futebol',
            newsletter: 'Não',
            contract: true,
            colors: [],
        }
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin: 60px;
}
</style>
