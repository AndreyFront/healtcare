<template>
    <div class="header">
        <div class="main-container max-width">
            <Logo />
            <div class="header__wrap-nav">
                <Nav :links="dataNav" />
                <button type="button" class="btn btn--theme--primary">
                    <span class="btn__text">Get Started</span>
                </button>
            </div>
        </div>
    </div>
</template>

<script>
import Logo from '@/ui/Logo'
import Nav from '@/components/Nav'

export default {
    name: 'Header',
    components: {
        Logo,
        Nav
    },
    data() {
        return {
            dataNav: [
                {
                    id: 1,
                    name: 'Home',
                    href: '/'
                },
                {
                    id: 2,
                    name: 'About',
                    href: '/about'
                },
                {
                    id: 3,
                    name: 'Article',
                    href: '/article'
                },
                {
                    id: 4,
                    name: 'Services',
                    href: '/services'
                }
            ]
        }
    }
}
</script>