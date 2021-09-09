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
    Ginger beer   
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 4 - Name the largest city on New Zealand's South Island?

  <label>
    Wellington
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Christchurch
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Palmerston    
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 5 - Name the highest mountain in New Zealand?

  <label>
    Mt Cook
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Mt Everest
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Mt Isobel    
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 6 - The Maori name for New Zealand is ‘Aotearoa’, what is the translation of this word?

  <label>
    New Zealand
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    The land of the long white cloud
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Long white cloud   
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 7 - What are the only land mammals native to New Zealand - all the others were introduced by Maoris and Europeans?
 
   <label>
    Kiwi
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Pokeko
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Moa  
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 8 - What's New Zealand's biggest city?

  <label>
    Christchurch
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Auckland
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    Wellington   
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 9 - What's the total population of New Zealand, as of 2021 September?

  <label>
    4.8 Million
    <input type="radio" bind:group={response} value={'yes'}>
    </label>

  <label>
    5.0 Million
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    5.01 Million 
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <button on:click={check(response)}> Check </button>

  <p>
    {result}
    </p>

Question 10 - What is the nickname given to New Zealanders?

  <label>
    Zealander's
    <input type="radio" bind:group={response} value={'no1'}>
    </label>

  <label>
    Newlander's
    <input type="radio" bind:group={response} value={'no2'}>
    </label>

  <label>
    Kiwi's 
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