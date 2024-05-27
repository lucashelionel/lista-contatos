<template>
    <div class="w-full px-2">
        <ListItem>
            João da Silva
            <template #actions>
                <button>Editar</button>
                <button>Excluir</button>
            </template>
        </ListItem>
    </div>

    <UIButton @click="addContact">Adicionar contato</UIButton>
</template>

<script setup>
const router = useRouter();//usado para fazer a navegação 
const addContact = () => {
    router.push('/form');
}

</script>