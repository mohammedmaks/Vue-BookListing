<template>
    <div>
        <h1>{{ title }}</h1>
        <ul>
            <li>{{ book.title }}: {{ book.author }}</li>
            <li v-for="book in books">{{ book.title }}: {{ book.author }}</li>
        </ul>
    </div>
</template>


<script>
export default {
    name: 'BookItem',
    props: ['book'],
};

</script>

<style>
li {
    display: block;
    margin: 0 10px;
}
</style>