<script>
  let name =''
  let age = 0
  let result = '';
	let response = ''
 	let points = ''
	
	function check(response) {
		if (response.includes('yes')) {
		result = 'correct'
		points += 1
		} else if (response.includes('no')) {
		result = 'wrong'
		} 
	}
	
  </script>
<main>
<h1>NZ General Knowlage Quiz!</h1>

<main>
<label>
Name:
  <input type="text" bind:value={name}>
  </label>
  
  <label>
  Age:
  <input type="number" bind:value={age}>
  </label>
  <button on:click={begin}>
    Enter
  </main>

  Question 1 - Which city is nicknamed the Edinburgh of the South?
  <label>
    Christchurch
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
     Dunedin
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Queenstown
    <input type="radio" bind:group={response} value={'no3'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>


Question 2 - Which New Zealand film maker and screenwriter won an Oscar for Best Director in 2003?

  <label>
    Taika Waititi
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Jane Campion
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <label>
    Jackson Peters    
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 3 - What famous fizzy drink was made in New Zealand?


  <label>
    L&P
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Coke
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Jackson Peters    
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>



<p>
	{points} points in total
</p>
</main>