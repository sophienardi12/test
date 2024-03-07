<script>
	export let image
	export let titolo
	export let descrizione
	export let prezzo
	export let button
</script>
 <!-- card_Pizze -->
    <div class="Card_pizze">
      <div class="card_pizze__img">
        <img src={image} alt="" />
      </div>
      <div class="card_pizze__centro">
        <p>{titolo}</p>
        <p class="Card_pizze__descrizione">{descrizione}</p>
      </div>
      <div class="Card_pizze__footer">
        <p>{prezzo}</p>
		 <div class="Card_pizze__button">
        <p>{button}</p>
		 </div>
   </div>
</div>

<style>
	
 .Card_pizze {
        background-color: #D7CBCB;
        width: 300px;
        border-radius: 20px;
        padding: 30px;
        font-style: normal;
        font-size: 20px;
        color: rgba(0, 0, 0, 0);
      }
	.card_pizze__img { 
        color: rgba(0, 0, 0, 0);
        height: 260px;
        object-fit: cover;
        aspect-ratio: 1;}

	.card_pizze__centro {color: rgba(0, 0, 0, 0);}

	.Card_pizze__descrizione {
        color: rgba(0, 0, 0, 0);
		font-size: 20px;
		font-style: italic
	}

	.Card_pizze__footer {
        color: rgba(0, 0, 0, 0);
		 display: flex;
     flex-direction: row;
     justify-content: space-between;
	}
 
	.Card_pizze__button { 
		border-radius: 11px;
        color: rgba(0, 0, 0, 0);
    background: #E38416;
	  width: 119.565px;
    height: 24px;
    flex-shrink: 0;}

	
</style>