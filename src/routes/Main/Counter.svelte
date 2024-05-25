
<!-- Counting logic -->

<script>
    import { onMount } from 'svelte';
    export let target = 0;
    export let duration = 3000;
  
    let value = 0;
    const interval = 10; // Milisegundos entre cada incremento
    const steps = Math.ceil(duration / interval);
    const step = target / steps;
  
    function startCounting() {
      const counter = setInterval(() => {
        value += step;
        if (value >= target) {
          value = target;
          clearInterval(counter);
        }
      }, interval);
    }
  
    onMount(() => {
      startCounting();
    });
  </script>

<style>
    .counter {
      font-size: 2em;
      text-align: center;
      padding: 10px;
      display: inline-block;
    }
  </style>
  
  <div class="counter">{Math.round(value)}</div>