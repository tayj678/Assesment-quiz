<script>
  let name =''
  let age = 0
  let result = ''
  let result1 = ''
  let result2 = ''
  let reslut3 = ''
  let reslut4 = ''
  let result5 =''
  let result6 = ''
  let reslut7 = ''
  let result8 = ''
  let result9 = ''
  let result10 = ''
	let response1 = ''
  let response2 = ''
  let response3 = ''
  let response4 = ''
  let response5 = ''
  let response6 = ''
  let response7 = ''
  let response8 = ''
  let response9 = ''
  let response10 = ''
 	let points = 0
	
function check(response) {
		if (response.includes('yes')) {
		result = 'correct'
		points += 1
		} else if (response.includes('no')) {
		result = 'wrong'
		} 


    if (response.includes('Q1')){
      result1 = result
    } else if (response.includes('Q2'))
      result2 = result
      result3 = result
      reslut4 = reslut
      result5 = result
      reslut6 = reslut
      reslut7 = reslut
      result8 = reslut
      result9 = reslut
      result10 = reslut 
	}

function begin(){
  
}
	
  </script>

  <h1>NZ General Knowlage Quiz</h1>


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
  </button><br>

 
  Question 1 - Which city is nicknamed the Edinburgh of the South? <br>
  <label>
    Christchurch
    <input type="radio" bind:group={response1} value={'Q1no1'}>
    </label>

  <label>
     Dunedin
    <input type="radio" bind:group={response1} value={'Q1yes'}>
    </label>

  <label>
    Queenstown
    <input type="radio" bind:group={response1} value={'Q1no3'}>
    </label>

  <button on:click={check(response1)}> Check </button>

  <p>
    {result1}
    </p>


Question 2 - Which New Zealand film maker and screenwriter won an Oscar for Best Director in 2003? <br>

  <label>
    Taika Waititi
    <input type="radio" bind:group={response2} value={'Q2no1'}>
    </label>

  <label>
    Jane Campion
    <input type="radio" bind:group={response2} value={'Q2no2'}>
    </label>

  <label>
    Jackson Peters    
    <input type="radio" bind:group={response2} value={'Q2yes'}>
    </label>

  <button on:click={check(response2)}> Check </button>

  <p>
    {result2}
    </p>

Question 3 - What famous fizzy drink was made in New Zealand? <br>


  <label>
    L&P
    <input type="radio" bind:group={response3} value={'yes'}>
    </label>

  <label>
    Coke
    <input type="radio" bind:group={response3} value={'no1'}>
    </label>

  <label>
    Ginger beer   
    <input type="radio" bind:group={response3} value={'no2'}>
    </label>

  <button on:click={check(response3)}> Check </button>

  <p>
    {result3}
    </p>

Question 4 - Name the largest city on New Zealand's South Island? <br>

  <label>
    Wellington
    <input type="radio" bind:group={response4} value={'no1'}>
    </label>

  <label>
    Christchurch
    <input type="radio" bind:group={response4} value={'yes'}>
    </label>

  <label>
    Palmerston    
    <input type="radio" bind:group={response4} value={'no2'}>
    </label>

  <button on:click={check(response4)}> Check </button>

  <p>
    {reslut4}
    </p>

Question 5 - Name the highest mountain in New Zealand? <br>

  <label>
    Mt Cook
    <input type="radio" bind:group={response5} value={'yes'}>
    </label>

  <label>
    Mt Everest
    <input type="radio" bind:group={response5} value={'no1'}>
    </label>

  <label>
    Mt Isobel    
    <input type="radio" bind:group={response5} value={'no2'}>
    </label>

  <button on:click={check(response5)}> Check </button>

  <p>
    {result5}
    </p>

Question 6 - The Maori name for New Zealand is ‘Aotearoa’, what is the translation of this word? <br>

  <label>
    New Zealand
    <input type="radio" bind:group={response6} value={'no1'}>
    </label>

  <label>
    The land of the long white cloud
    <input type="radio" bind:group={response6} value={'yes'}>
    </label>

  <label>
    Long white cloud   
    <input type="radio" bind:group={response6} value={'no2'}>
    </label>

  <button on:click={check(response6)}> Check </button>

  <p>
    {result6}
    </p>

Question 7 - What are the only land mammals native to New Zealand - all the others were introduced by Maoris and Europeans? <br>
 
   <label>
    Kiwi
    <input type="radio" bind:group={response7} value={'no1'}>
    </label>

  <label>
    Pokeko
    <input type="radio" bind:group={response7} value={'yes'}>
    </label>

  <label>
    Moa  
    <input type="radio" bind:group={response7} value={'no2'}>
    </label>

  <button on:click={check(response7)}> Check </button>

  <p>
    {result7}
    </p>

Question 8 - What's New Zealand's biggest city? <br>

  <label>
    Christchurch
    <input type="radio" bind:group={response8} value={'no1'}>
    </label>

  <label>
    Auckland
    <input type="radio" bind:group={response8} value={'yes'}>
    </label>

  <label>
    Wellington   
    <input type="radio" bind:group={response8} value={'no2'}>
    </label>

  <button on:click={check(response8)}> Check </button>

  <p>
    {result8}
    </p>

Question 9 - What's the total population of New Zealand, as of 2021 September? <br>

  <label>
    4.8 Million
    <input type="radio" bind:group={response9} value={'yes'}>
    </label>

  <label>
    5.0 Million
    <input type="radio" bind:group={response9} value={'no1'}>
    </label>

  <label>
    5.01 Million 
    <input type="radio" bind:group={response9} value={'no2'}>
    </label>

  <button on:click={check(response9)}> Check </button>

  <p>
    {result9}
    </p>

Question 10 - What is the nickname given to New Zealanders? <br>

  <label>
    Zealander's
    <input type="radio" bind:group={response10} value={'no1'}>
    </label>

  <label>
    Newlander's
    <input type="radio" bind:group={response10} value={'no2'}>
    </label>

  <label>
    Kiwi's 
    <input type="radio" bind:group={response10} value={'yes'}>
    </label>

  <button on:click={check(response10)}> Check </button>

  <p>
    {result10}
    </p> 

<p>
	{points} points in total
</p>
