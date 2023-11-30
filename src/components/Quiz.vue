<template>
    <div class="alert alert-success">
        <h2>クイズを作ります</h2>
        <p>{{ quiz_text }}</p>
    </div>
</template>
<script>
// JSで外部のファイルから呼び出せる状態を表す
export default {
    name: 'Quiz',
    props: {
        quiz_text: String
    }
}
</script>
