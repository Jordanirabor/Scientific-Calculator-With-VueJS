<template>

<div @click="buttonClick">

<button class="btn btn-primary">7</button>
<button class="btn btn-primary">8</button>
<button class="btn btn-primary">9</button>
<button class="btn btn-primary">/</button>
<button class="btn btn-primary">&larr;</button>
<button class="btn btn-primary">C</button>
<button class="btn btn-primary">4</button>
<button class="btn btn-primary">5</button>
<button class="btn btn-primary">6</button>
<button class="btn btn-primary">*</button>
<button class="btn btn-primary"> ( </button>
<button class="btn btn-primary"> ) </button>
<button class="btn btn-primary">1</button>
<button class="btn btn-primary">2</button>
<button class="btn btn-primary">3</button>
<button class="btn btn-primary">-</button>
<button class="btn btn-primary">x²</button>
<button class="btn btn-primary">±</button>
<button class="btn btn-primary">0</button>
<button class="btn btn-primary">.</button>
<button class="btn btn-primary">%</button>
<button class="btn btn-primary">+</button>
<button class="equals btn btn-primary">=</button>

</div>

</template>

<script>

export default {

  data () {
    return {

    }
  },
  methods: {

      buttonClick: function(e){
        let value = e.target.innerText;
         this.$emit('addNumber', value) 
      }
    
    }
}
</script>

<style scoped>

button {
padding: 1.25em 2em;
margin: 1em 1.2em;
width: 68.45px;
height: 60px;
border: none;
background: #178;
}

.equals {
background: green;
margin: 1em;
border: none;
background: rgb(0, 150, 50);
padding: 1.25em 5.5em;
}

</style>
