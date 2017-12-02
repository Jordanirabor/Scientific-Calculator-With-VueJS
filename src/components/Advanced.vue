<template>

<div @click="buttonClick">

<button class="btn btn-primary">sin</button>
<button class="btn btn-primary">cos</button>
<button class="btn btn-primary">tan</button>
<button class="btn btn-primary">x^</button>
<button class="btn btn-primary">&larr;</button>
<button class="btn btn-primary">C</button>
<button class="btn btn-primary">log</button>
<button class="btn btn-primary">ln</button>
<button class="btn btn-primary">e</button>
<button class="btn btn-primary">∘</button>
<button class="btn btn-primary">rad</button>
<button class="btn btn-primary">√</button>
<button class="btn btn-primary">7</button>
<button class="btn btn-primary">8</button>
<button class="btn btn-primary">9</button>
<button class="btn btn-primary">/</button>
<button class="btn btn-primary">x²</button>
<button class="btn btn-primary">x!</button>
<button class="btn btn-primary">4</button>
<button class="btn btn-primary">5</button>
<button class="btn btn-primary">6</button>
<button class="btn btn-primary">*</button>
<button class="btn btn-primary">(</button>
<button class="btn btn-primary">)</button>
<button class="btn btn-primary">1</button>
<button class="btn btn-primary">2</button>
<button class="btn btn-primary">3</button>
<button class="btn btn-primary">-</button>
<button class="btn btn-primary">%</button>
<button class="btn btn-primary">+</button>
<button class="btn btn-primary">±</button>
<button class="btn btn-primary">0</button>
<button class="btn btn-primary">.</button>
<button class="btn btn-primary">&#x003C0;</button>
<button class="btn btn-primary">+</button>
<button class="btn btn-primary equals">=</button>



  </div>

</template>

<script>

export default {
  name: 'Advanced',
  data () {
    return {

    }
  },
  methods: {

     buttonClick: function(e){
        let value = e.target.innerHTML;
         this.$emit('addNumber', value) 
      }
  }
}
</script>

<style scoped>

button {
padding: 0.5em 2em;
margin: 1em 1.5em;
border: none;
width: 15px;
height: 35px;
text-align: center;
background: #178;
}

.equals {
background: rgb(0, 150, 50);
}

</style>
