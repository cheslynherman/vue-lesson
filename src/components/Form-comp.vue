<template>
   <h2>Text Input</h2>
   <input v-model="text"> {{text}}
   <h2>Checkbox</h2>
   <input type="checkbox" id="checkbox" v-model="checked">
   <label for="checkbox">Checked:{{checked}}</label>

   <h2>Multi Checkbox</h2>
   <input type="checkbox" id="cheslyn" v-model="checkedNames" value="Cheslyn">
   <label for="cheslyn">Cheslyn</label>

   <input type="checkbox" id="luke" v-model="checkedNames" value="Luke">
    <label for="luke">Luke</label>
    <p> Checked:
    <pre>{{checkedNames}}</pre>
    </p>

    <h2>Radio</h2>
    <input type="radio" id="one" value="one" v-model="picked">
    <label for="one">One</label>
    <br>
    <input type="radio" id="two" value="two" v-model="picked">
    <label for="two">Two</label>
    <br>
    <span>Picked: {{picked}}</span>

    <h2>Multi Selected</h2>
    <select v-model="multiSelected" multiple style="width:100px">
        <option>A</option>
        <option>B</option>
        <option>C</option>
        
    </select>
    <span>selected: {{multiSelected}}</span>
</template>


<script>
export default {
    data () {
        return {
            text: '', 
            checked: true,
            checkedNames: ['Cheslyn'], 
            picked: 'one',
            multiSelected: 'A',
        }
    }
}
</script>