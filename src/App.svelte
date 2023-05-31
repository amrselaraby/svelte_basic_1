<script>
 import Counter from './lib/Counter.svelte'
 const props = {
  maxCount: 10,
  initialCount: 5 
 };

 console.log($$props, $$restProps)
</script>

<Counter {...props}/>

<style>
  
</style>