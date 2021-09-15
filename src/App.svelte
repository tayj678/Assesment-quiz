<script>
	//these are all of the names of the variables that are used throughout my code. 
    let name = '';
		let formClass = '';
    let result = '';
    let result1 = '';
    let result2 = '';
    let result3 = '';
    let result4 = '';
    let result5 = '';
    let result6 = '';
    let result7 = '';
    let result8 = '';
    let result9 = '';
    let resultx = '';
		let response = '';
    let response1 = '';
    let response2 = '';
    let response3 = '';
    let response4 = '';
    let response5 = '';
    let response6 = '';
    let response7 = '';
    let response8 = '';
    let response9 = '';
    let responsex = '';
    let points = 0;
		let p = '';
		
// this is a fuction which checks if the answer choosen is correct or wrong. It also adds points when the player gets the questions correct. 
    function check(response) {
        if (response.includes("yes")) {
            result = "correct";
            points += 1;
        } else if (response.includes("no")) {
            result = "wrong";
        }

	// This makes sure that each question is checked induvidually wheither its right or wrong. Result is from the function above which see's if the player got the question right or wrong.  
    if (response.includes("Q1")) {
           result1 = result;
        } else if (response.includes("Q2")){
						result2 = result;
				} else if (response.includes("Q3")){
						result3 = result;
				} else if (response.includes("Q4")){
						result4 = result;
				} else if (response.includes('Q5')){
						result5 = result
				} else if (response.includes('Q6')){
						result6 = result
				} else if (response.includes('Q7')){
						result7 = result
				} else if (response.includes('Q8')){
						result8 = result
				} else if (response.includes('Q9')){
						result9 = result
				} else if (response.includes('Qx')){
						resultx = result
				}
		}
	// this function is for question 8 as it is a text question. There is a while loop which continously checks when someone does not write anything in the box, it will tell them to write something. It also has the same point system as the other function where if it is correct it will add a point and if it is wrong it will say "wrong".
		function check2(){
			while (response8 == ''){
		p = 'please enter your response'
	}
			if (response8 ==='Kaikoura'){
				result8 = 'correct'
				points += 1
			}else{
				result8 = 'wrong'
			}
		}
	
	// this function is for when the player finishes the quiz and wants to start again. The button at the bottom of the code will reset the points and reset the questions. 
		function reset(){
			points = 0
			response1 ='';
			response2 ='';
			response3 ='';
			response4 ='';
			response5= '';
			response6= '';
			response7= '';
			response8= '';
			response9= '';
			responsex= '';
}
			

</script>

<h1>NZ General Knowlage Quiz</h1>

<!-- this is a box which lets you write your name -->
<label>
  Name: 
  <input bind:value={name}> <br>
	<!-- this is a box which lets you write your form class -->
	Form Class:
	<input bind:value={formClass}>
</label>
	
<!-- this can put your name/form class in the curly brackets -->
<h1>Kia Ora {name}! {formClass}</h1>

	<!-- This is question one, whithin this there are three possible answers -->
Question 1 - Which city is nicknamed the Edinburgh of the South? <br />
<label>
    Christchurch
    <input type="radio" bind:group={response1} value={"Q1no1"} />
</label>

<label>
    Dunedin
    <input type="radio" bind:group={response1} value={"Q1yes"} />
</label>

<label>
    Queenstown
    <input type="radio" bind:group={response1} value={"Q1no3"} />
</label>

<button on:click={check(response1)}> Check </button>

<p>
    {result1}
</p>

	<!-- This is question two, whithin this there are three possible answers -->
Question 2 - Which New Zealand film maker and screenwriter won an Oscar for Best
Director in 2003?<br />

<label>
    Taika Waititi
    <input type="radio" bind:group={response2} value={"Q2no1"} />
</label>

<label>
    Jane Campion
    <input type="radio" bind:group={response2} value={"Q2no2"} />
</label>

<label>
    Jackson Peters
    <input type="radio" bind:group={response2} value={"Q2yes"} />
</label>

<button on:click={check(response2)}> Check </button>

<p>
    {result2}
</p>

	<!-- This is question three, whithin this there are three possible answers -->
Question 3 - What famous fizzy drink was made in New Zealand?<br />

<label>
    Lemon and Paeroa
    <input type="radio" bind:group={response3} value={"Q3yes"} />
</label>

<label>
    Coke
    <input type="radio" bind:group={response3} value={"Q3no1"} />
</label>

<label>
    Ginger beer
    <input type="radio" bind:group={response3} value={"Q3no2"} />
</label>

<button on:click={check(response3)}> Check </button>

<p>
    {result3}
</p>

	<!-- This is question four, whithin this there are three possible answers -->
Question 4 - Name the largest city on New Zealand's?<br />

<label>
    Wellington
    <input type="radio" bind:group={response4} value={"Q4no1"} />
</label>

<label>
    Auckland
    <input type="radio" bind:group={response4} value={"Q4yes"} />
</label>

<label>
    Christchurch
    <input type="radio" bind:group={response4} value={"Q4no2"} />
</label>

<button on:click={check(response4)}> Check </button>

<p>
    {result4}
</p>

	<!-- This is question five, whithin this there are three possible answers -->
Question 5 - Name the highest mountain in New Zealand?<br />

<label>
    Mt Cook
    <input type="radio" bind:group={response5} value={"Q5yes"} />
</label>

<label>
    Mt Everest
    <input type="radio" bind:group={response5} value={"Q5no1"} />
</label>

<label>
    Mt Isobel
    <input type="radio" bind:group={response5} value={"Q5no2"} />
</label>

<button on:click={check(response5)}> Check </button>

<p>
    {result5}
</p>

	<!-- This is question six, whithin this there are three possible answers -->
Question 6 - The Maori name for New Zealand is ‘Aotearoa’, what is the
translation of this word?<br />

<label>
    New Zealand
    <input type="radio" bind:group={response6} value={"Q6no1"} />
</label>

<label>
    The land of the long white cloud
    <input type="radio" bind:group={response6} value={"Q6yes"} />
</label>

<label>
    Long white cloud
    <input type="radio" bind:group={response6} value={"Q6no2"} />
</label>

<button on:click={check(response6)}> Check </button>

<p>
    {result6}
</p>

	<!-- This is question seven, whithin this there are three possible answers -->
Question 7 - What are the only land mammals native to New Zealand - all the
others were introduced by Maoris and Europeans?<br />

<label>
    Kiwi
    <input type="radio" bind:group={response7} value={"Q7yes"} />
</label>

<label>
    Pukeko
    <input type="radio" bind:group={response7} value={"Q7no1"} />
</label>

<label>
    Moa
    <input type="radio" bind:group={response7} value={"Q7no2"} />
</label>

<button on:click={check(response7)}> Check </button>

<p>
    {result7}
</p>

	<!-- This is question eight, whithin this there are three possible answers -->
Question 8 - What's the town known for the best Fish 'n' Chips?<br />

<label>
    <input type="text" bind:value={response8} placeholder= 'enter answer' />
</label>

<button on:click={check2(response8)}> Check </button>

<p>
	{p}
</p>

<p>
    {result8}
</p>

	<!-- This is question nine, whithin this there are three possible answers -->
Question 9 - What's the total population of New Zealand, as of 2021 September?<br
/>

<label>
    4.8 Million
    <input type="radio" bind:group={response9} value={"Q9yes"} />
</label>

<label>
    5.0 Million
    <input type="radio" bind:group={response9} value={"Q9no1"} />
</label>

<label>
    5.01 Million
    <input type="radio" bind:group={response9} value={"Q9no2"} />
</label>

<button on:click={check(response9)}> Check </button>

<p>
    {result9}
</p>

	<!-- This is question ten, whithin this there are three possible answers -->
Question 10 - What is the nickname given to New Zealanders?<br />

<label>
    Zealanders
    <input type="radio" bind:group={responsex} value={"Qxno1"} />
</label>

<label>
    Newlanders
    <input type="radio" bind:group={responsex} value={"Qxno2"} />
</label>

<label>
    Kiwis
    <input type="radio" bind:group={responsex} value={"Qxyes"} />
</label>

<button on:click={check(responsex)}> Check </button>

<p>
    {resultx}
</p>

<!-- -->
<p>
    {points} points in total
</p>

<!-- -->
<button on:click={reset}>
  Reset & Go to Top
</button>