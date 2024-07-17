<script>
export default {
    name: 'EquipeView',
    data() {
        return {
            equipe: [
               {
                    nome: 'Eduardo Bomsenhor',
                    cargo: 'Desenvolvedor {'
                },
                {
                    nome: 'Henrique Dias Belboni',
                    cargo: 'Desenvolvedor {'
                }, 
                {
                    nome: 'Gabrieli Marta',
                    cargo: 'Desenvolvedor {'
                },
                {
                    nome: 'Davi da Rosa',
                    cargo: 'Designer'
                },
                {
                    nome: 'Vallentini',
                    cargo: 'Gerente de Projetos'
                },
                {
                     nome: 'Marco Peruzzo',
                     cargo: 'Designer'
                }
            ]
        }
    }
}
</script>

<template>
    <div>
        <h1>Equipe</h1>
        <ul>
            <li v-for="membro in equipe" :key="membro.nome">
                <h2>{{ membro.nome }}</h2>
                <p>{{ membro.cargo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
/* Your component-specific styles go here */
</style>