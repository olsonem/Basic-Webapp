# test-project

> A Vue.js project

## Build Setup

``` bash
# install framework globaly
vue intuit -g vue-cli

# bootstrap the application
npm install webpack test-project

# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# modify the app
src/components/Hello.vue

# change the content in the <template>
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>2 Things that are difficult in JavaScript</h2>
    <ol>
      <li>naming things</li>
      <li>recursion</li>
      <li>off-by-one errors</li>
    </ol>
  </div>
</template>

# alter the <style> to create an ordered list
<style scoped>
h1, h2 {
  font-weight: normal;
}

ol {
  list-style-type: decimal;
  width: 40%;
  margin: auto;
}

li {
  display: list-item;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>

# add content data objects to the <script>
<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'This Data Has Been Altered',
      num1: 42,
      num2: 78
    }
  }
}
</script>

# add a method to the <script>
  methods: {
    calculateProduct: function(){
      this.product = this.num1 * this.num2;
    }

# add the object reference to the <template>
  <p>What is {{ num1 }} times {{ num2 }}?</p>

# add an event listener to the <template>
<p>What is {{ num1 }} times {{ num2 }}?<span v-if="product">{{ product }}</span></p>
<button v-on:click="calculateProduct">Calculate</button>

# add an addition data object for the product in the <script>
product: null

# install Vue-Devtools on your browser and use the inspect feature to check for syntax and logic errors

# create a github repository for this project 

# initialize git
init git

# add the files 
git add -A

# commit the files with a comment
git commit -m "this is a comment"

# add the remote origin on github
git remote add origin git@github.com:githubname/reponame.git

# push the files to a git hub
git push -u origin

# configure webpack in the config/index.js file by changing "dist" to "docs"
index: path.resolve(__dirname, '../docs/index.html'),
assetsRoot: path.resolve(__dirname, '../docs'),

# set the assetsPublicPath to ' '
assetsPublicPath: '',

# build for production and view the bundle analyzer report
npm run build --report

#configure github pages by setting the source to "master branch /docs folder"



```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
