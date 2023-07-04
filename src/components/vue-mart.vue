<script src="https://npmcdn.com/vue/dist/vue.js"></script>
<div id="app">
 {{ message }}
</div>
<script>
new Vue({
 el: '#app',
 data: {
 message: 'Hello Vue.js!'
 }
})
</script>
<script>
export default {
  name: 'vue-mart'
}
</script>