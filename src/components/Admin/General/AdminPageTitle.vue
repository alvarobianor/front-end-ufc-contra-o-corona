<template>
    <div class="admin-page-title">
        <h1 class="admin-page-title__main">{{ title }}</h1>
        <h2 class="admin-page-title__sub">
            <slot></slot>
        </h2>
    </div>
</template>

<script>
export default {
    name: 'AdminPageTitle',
    props: {
        title: {
            type: String,
            required: true
        }
    }
}
</script>

<style lang="scss" scoped>
.admin-page-title {
    &__main {
        font-size: 3.6rem;
        font-weight: 700;
        line-height: 3.6rem;
        color: rgba($black, 0.87);
    }

    &__sub {
        font-size: 1.8rem;
        font-weight: 400;
        color: rgba($black, 0.45);
    }
}
</style>
