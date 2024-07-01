
<template>
    <div class="card">
        <Menubar :model="items" />
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [
                {
                    label: 'Início',
                    icon: 'pi pi-home',
                    command:()=>{
                            this.$router.push('/')
                        }
                },
                {
                    label: 'Sobre',
                    icon: 'pi pi-info-circle',
                    command:()=>{
                            this.$router.push('/about')
                        }
                },
                {
                    label: 'Contato',
                    icon: 'pi pi-envelope',
                    command:()=>{
                            this.$router.push('/contact')
                        }
                },
                {
                    label: 'Entrar',
                    icon: 'pi pi-sign-in',
                    command:()=>{
                            this.$router.push('/login')
                        }
                },
                {
                    label: 'Criar conta',
                    icon: 'pi pi-user-plus',
                    command:()=>{
                            this.$router.push('/register')
                        }
                }
            ]
        };
    }
};
</script>

<style scoped>
    :deep(.p-menubar){
        background-color: transparent !important;
        border: none !important;
    }
</style>
