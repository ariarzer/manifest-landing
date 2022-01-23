<script>
	export let name;
	import Header from './components/Header.svelte';
	import Article from './components/Article.svelte';
	import Slides from './components/Slides.svelte';
	import BigSlide from './components/BigSlide.svelte';
	import LabeledSlide from './components/LabeledSlide.svelte';
	import SalaryPrice from './components/SalaryPrice.svelte';
	import Radio from './components/Radio.svelte';
	import Applications from './components/Applications.svelte';
	import Badge from './components/Badge.svelte';
	import DetailsItem from './components/DetailsItem.svelte';
</script>

<Header/>

<main class="Content">
	<Article class="Article--howToEarn">
		<span slot="image">🪙</span>
		<span slot="header">Как зарабатывать в Манифесте?</span>
		<Slides modificator="howToEarn">
			<BigSlide>
				<h3>Скачайте приложение</h3>
				<p>Доступно на обеих платформах.</p>
			</BigSlide>
			<BigSlide>
				<h3>Подключите Instagram</h3>
				<p>Это абсолютно безопасно.</p>
			</BigSlide>
			<BigSlide>
				<h3>Участвуйте в кампаниях</h3>
				<p>Продвигайте любимые бренды.</p>
			</BigSlide>
		</Slides>
	</Article>

	<Article>
		<span slot="image">👀</span>
		<span slot="header">В каких кампаниях можно участвовать?</span>
		<Radio/>
		<Slides modificator="companies">
			<LabeledSlide>
				<div slot="topBadge">Он такой один</div>
				<div slot="bottomBadge">
					<SalaryPrice>
						<span slot="oldPrice">500 ₽</span>
						<span slot="newPrice">600 ₽</span>
					</SalaryPrice>
				</div>
				<span slot="label">Он такой один</span>
				<span slot="secondaryLabel">Тинькофф</span>
			</LabeledSlide>
			<LabeledSlide>
				<div slot="topBadge">Он такой один</div>
				<div slot="bottomBadge">
					<SalaryPrice>
						<span slot="oldPrice">500 ₽</span>
						<span slot="newPrice">600 ₽</span>
					</SalaryPrice>
				</div>
				<span slot="label">Он такой один</span>
				<span slot="secondaryLabel">Тинькофф</span>
			</LabeledSlide>
			<LabeledSlide>
				<div slot="topBadge">Он такой один</div>
				<div slot="bottomBadge">
					<SalaryPrice>
						<span slot="oldPrice">500 ₽</span>
						<span slot="newPrice">600 ₽</span>
					</SalaryPrice>
				</div>
				<span slot="label">Он такой один</span>
				<span slot="secondaryLabel">Тинькофф</span>
			</LabeledSlide>
			<LabeledSlide>
				<div slot="topBadge">Он такой один</div>
				<div slot="bottomBadge">
					<SalaryPrice>
						<span slot="oldPrice">500 ₽</span>
						<span slot="newPrice">600 ₽</span>
					</SalaryPrice>
				</div>
				<span slot="label">Он такой один</span>
				<span slot="secondaryLabel">Тинькофф</span>
			</LabeledSlide>
		</Slides>
		<h3>Участвуйте в crowd-promotion кампаниях. Здесь вы сразу видите сумму заработка и получаете ее через
			24 часа после публикации сторис или поста.
		</h3>
		<p>В CPM кампаниях всегда яркие интерактивные маски,
			которые точно понравятся твоей аудитории.</p>
		<Applications/>
	</Article>

	<Article>
		<span slot="image">🤩</span>
		<span slot="header">Почему именно манифест?</span>
		<Slides modificator="why">
			<BigSlide>
				<h3>Быстрые выплаты</h3>
				<p>В течение суток. Выбор из разных способов вывода.</p>
			</BigSlide>
			<BigSlide>
				<h3>Яркие креативы</h3>
				<p>Крутые форматы, которые понравятся вашим подписчикам.</p>
			</BigSlide>
			<BigSlide>
				<h3>Быстро и без бюрократии</h3>
				<p>На размещение рекламы уходит 5 минут. Без долгих согласований.</p>
			</BigSlide>
		</Slides>
	</Article>

	<Article>
		<span slot="image">📖</span>
		<span slot="header">А еще мы публикуем образовательный контент!</span>
		<Slides modificator="education">
			<BigSlide>
				<p>Как делать reels, которые станут виртуальными?</p>
			</BigSlide>
			<BigSlide>
				<p>Как делать reels, которые станут виртуальными?</p>
			</BigSlide>
			<BigSlide>
				<p>Как делать reels, которые станут виртуальными?</p>
			</BigSlide>
			<BigSlide>
				<p>Как делать reels, которые станут виртуальными?</p>
			</BigSlide>
			<BigSlide>
				<p>Как делать reels, которые станут виртуальными?</p>
			</BigSlide>
		</Slides>
		<h3>В Манифесте вы можете не только зарабатывать, но и развивать свой аккаунт, чтобы сумма вознаграждений увеличивалась вместе с ростом подписчиков.</h3>
		<p>В приложении вы найдете полезные материалы, которые помогут повысить
			качество контента и увеличить количество подписчиков.</p>
		<h3>Вместе с нами уже выросли:</h3>
		<Slides modificator="withUs">
			<BigSlide>
				<Badge>+ 16 843 ₽</Badge>
				<h3>Даша</h3>
				<p>Было — 272 ₽.<br>Стало — 17 115 ₽.</p>
			</BigSlide>
			<BigSlide>
				<Badge>+ 16 843 ₽</Badge>
				<h3>Наташа</h3>
				<p>Было — 6 574 ₽. <br>Стало — 18 782 ₽.</p>
			</BigSlide>
			<BigSlide>
				<Badge>+ 16 843 ₽</Badge>
				<h3>Вероника</h3>
				<p>Было — 6 574 ₽. <br>Стало — 18 782 ₽.</p>
			</BigSlide>
		</Slides>
		<h3>Хотите так же или еще лучше?
			Устанавливайте приложение Манифест.</h3>
		<Applications/>

	</Article>

	<Article>
		<span slot="image">🤔</span>
		<span slot="header">Ваши вопросы - наши ответы</span>
		<DetailsItem>
			<summary><h3>Какая цель у Манифеста?</h3></summary>
			<p>Манифест — это платформа, которая способствует творчеству. Мы вознаграждаем творческих людей и
				пользователей. Перед размещением поста вы получаете солидное денежное предложение. Вы получите оплату
				в течение 24 часов.</p>
		</DetailsItem>
		<DetailsItem>
			<summary><h3>Какая цель у Манифеста?</h3></summary>
			<p>Манифест — это платформа, которая способствует творчеству. Мы вознаграждаем творческих людей и
				пользователей. Перед размещением поста вы получаете солидное денежное предложение. Вы получите оплату
				в течение 24 часов.</p>
		</DetailsItem>
		<DetailsItem>
			<summary><h3>Какие способы вывода существуют?</h3></summary>
			<p>Манифест — это платформа, которая способствует творчеству. Мы вознаграждаем творческих людей и
				пользователей. Перед размещением поста вы получаете солидное денежное предложение. Вы получите оплату
				в течение 24 часов.</p>
		</DetailsItem>
	</Article>
</main>

<style>
	main {
		position: relative;
		display: flex;
		flex-direction: column;
		padding: 0 300px;
		box-sizing: border-box;
		gap: 120px;
	}
	main::before {
		content: '';
		height: 60px;
		width: 100%;
		display: block;
		border-radius: 60px 60px 0 0;
		position: absolute;
		top: -60px;
		left: 0;
		background-color: white;
	}
</style>
