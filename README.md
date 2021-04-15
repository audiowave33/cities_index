# cities_index
Lumen (8.2.3)
api для сайта индекс-городов.рф


		<h4>Получить весь список городов</h4>
		<p><br>GET</br>http://audiowave33.ru/api/city</p>

	</div>
	<div>
		<h4>Найти город по id</h4>
		<p><br>GET</br>http://audiowave33.ru/api/city/id</p>
		<p>Пример: http://audiowave33.ru/api/city/5</p>
	</div>
	<div>
		<h4>Случайный город</h4>
		<p><br>GET</br>http://audiowave33.ru/api/city/random</p>
	</div>
	<div>
		<h4>Поиск города</h4>
		<p><br>POST</br>http://audiowave33.ru/api/city/search</p>
		<p><b>Параметры запроса:</b></p>
		<p>name - название города</p>
		<p>region - название округа или области</p>
		<p>Пример №1: http://audiowave33.ru/api/city/search<br>
			name: Тюмень</p>
		<p>Пример №2: http://audiowave33.ru/api/city/search<br>
			region: Амурская область</p>
	</div>
