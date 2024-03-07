<script lang="ts">
	import CardPizza from '$components/CardPizza.svelte';

	let pizze = [
		{
			titolo: 'Pizza Margherita',
			descrizione:
				'composta da una base di pasta lievitata, generosamente condita con salsa di pomodoro fresca e leggera. Il tocco cremoso è dato dalla mozzarella, un formaggio a pasta filata, che si fonde splendidamente con il calore del forno.',
			prezzo: '7 euro',
			button: 'Add to cart',
			image:
				'https://it.ooni.com/cdn/shop/articles/Margherita-9920.jpg?crop=center&height=800&v=1644590028&width=800'
		},
		{
			titolo: 'Pizza Diavola',
			descrizione:
				'condita con salsa di pomodoro leggermente piccante, mozzarella cremosa e fette di salame piccante che aggiungono un tocco di sapore intenso. ',
			prezzo: '7 euro',
			button: 'Add to cart',
			image: 'https://img.cuisineaz.com/660x660/2022/06/30/i184454-pizza-diavola.jpeg'
		},
		{
			titolo: 'Pizza 4 formaggi',
			descrizione:
				'mozzarella, gorgonzola, fontina e parmigiano reggiano, creando un mix di sapori cremosi, piccanti e intensi ',
			prezzo: '7 euro',
			button: 'Add to cart',
			image:
				'https://uploads-ssl.webflow.com/6001804d7e7aa9837e4eec83/6421b870c3a0c85a9d35a3f2_quattro-fromaggi-pizza.jpg'
		},
		{
			titolo: 'Pizza speciale',
			descrizione:
				"prosciutto, funghi, peperoni, olive, cipolle, carciofi, salsiccia. creando un mix di sapori cremosi, piccanti e intensi che rendono questa pizza un'esperienza irresistibile per gli amanti del formaggio.",
			prezzo: '7 euro',
			button: 'Add to cart',
			image:
				'https://www.soniaperonaci.it/wp-content/uploads/2022/02/Pizza-con-mortadella-burrata-e-pesto-di-pistacchi-5.jpg'
		}
	];
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tailwindcss@3.4.1/src/css/preflight.css" />
</svelte:head>

{#each pizze as pizza}
	<CardPizza
		titolo={pizza.titolo}
		descrizione={pizza.descrizione}
		prezzo={pizza.prezzo}
		button={pizza.button}
		image={pizza.image}
	/>
{/each}
