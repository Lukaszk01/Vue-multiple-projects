<template>
  <div id="app">
    <Header />

    <b-container class="bv-example-row">
      <b-row>
        <b-col sm="6" offset="3">
          <QuestionBox
            :currentQuestion="questions[index]"
          />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import QuestionBox from './components/QuestionBox.vue'
export default {
  name: 'app',
  components: {
    Header,
    QuestionBox
    // :currentQuestion="questions[index]"
  },
  data() {
    return {
      questions: [],
      index: 0
    },
[
  {"category":"Animals","type":"multiple","difficulty":"medium","question":"What color colour is a polar bear&#039;s skin?","correct_answer":"Black","incorrect_answers":["White","Pink","Green"]}
  ,{"category":"Animals","type":"multiple","difficulty":"easy","question":"How many legs do butterflies have?","correct_answer":"6","incorrect_answers":["2","4","0"]}
  ,{"category":"Animals","type":"multiple","difficulty":"hard","question":"How many known living species of hyenas are there?","correct_answer":"4","incorrect_answers":["8","2","6"]},
  {"category":"Animals","type":"multiple","difficulty":"medium","question":"Which animal was part of an Russian domestication experiment in 1959?","correct_answer":"Foxes","incorrect_answers":["Pigeons","Bears","Alligators"]},
  {"category":"Animals","type":"multiple","difficulty":"hard","question":"What type of creature is a Bonobo?","correct_answer":"Ape","incorrect_answers":["Lion","Parrot","Wildcat"]},
  {"category":"Animals","type":"multiple","difficulty":"medium","question":"What is the name of the family that the domestic cat is a member of?","correct_answer":"Felidae","incorrect_answers":["Felinae","Felis","Cat"]},
  {"category":"Animals","type":"multiple","difficulty":"medium","question":"What dog bread is one of the oldest breeds of dog and has flourished since before 400 BCE.","correct_answer":"Pugs","incorrect_answers":["Bulldogs","Boxers","Chihuahua"]},
  {"category":"Animals","type":"multiple","difficulty":"hard","question":"What is the name of the copper-rich protein that creates the blue blood in the Antarctic octopus?","correct_answer":"Hemocyanin","incorrect_answers":["Cytochrome","Iron","Methionine"]},
  {"category":"Animals","type":"multiple","difficulty":"medium","question":"What is the collective noun for rats?","correct_answer":"Mischief","incorrect_answers":["Pack","Race","Drift"]},
{"category":"Animals","type":"multiple","difficulty":"medium","question":"&quot;Decapods&quot; are an order of ten-footed crustaceans.  Which of these are NOT decapods?","correct_answer":"Krill","incorrect_answers":["Lobsters","Shrimp","Crabs"]}]}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
