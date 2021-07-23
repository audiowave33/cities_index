# cities_index
Lumen (8.2.3)
api для сайта индекс-городов.рф
<div>
		<h4>Получить весь список городов</h4>
		<p><br>GET</br>http://audiowave33.ru/cityapi/public/api</p>
		<p>Результат: 
[<br>
    {<br>
        "id": 1,<br>
        "name": "Красновишерск",<br>
        "region": "Пермский край",<br>
        "size": "Малый город",<br>
        "climat": "условно комфортный климат",<br>
        "population": "14,8 тыс.чел.",<br>
        "points": 169,<br>
        "residential and adjacent spaces": 39,<br>
        "street networks": 30,<br>
        "green spaces": 22,<br>
        "public and business infrastructure and adjacent spaces": 21,<br>
        "social and leisure infrastructure and adjacent spaces": 20,<br>
        "citywide space": 37,<br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/3670/thumb_327_krasnovishersk.png"<br>
    },<br>
    {<br>
        "id": 2,<br>
        "name": "Касли",<br>
        "region": "Челябинская область",<br>
        "size": "Малый город",<br>
        "climat": "условно комфортный климат",<br>
        "population": "15,7 тыс.чел.",<br>
        "points": 168,<br>
        "residential and adjacent spaces": 30,<br>
        "street networks": 30,<br>
        "green spaces": 23,<br>
        "public and business infrastructure and adjacent spaces": 27,<br>
        "social and leisure infrastructure and adjacent spaces": 25,<br>
        "citywide space": 33,<br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/3612/thumb_268_Kasli_2002.png"<br>
    },<br>
    {<br>
        "id": 3,<br>
        "name": "Костерево",<br>
        "region": "Владимирская область",<br>
        "size": "Малый город",<br>
        "climat": "условно комфортный климат",<br>
        "population": "8,1 тыс.чел.",<br>
        "points": 172,<br>
        "residential and adjacent spaces": 32,<br>
        "street networks": 31,<br>
        "green spaces": 23,<br>
        "public and business infrastructure and adjacent spaces": 26,<br>
        "social and leisure infrastructure and adjacent spaces": 21,<br>
        "citywide space": 39,<br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/3659/thumb_316_kosterevo.png"<br>
    },...<br>
    И так далее</p>
	</div>
	<div>
		<h4>Найти город по id</h4>
		<p><br>GET</br>http://audiowave33.ru/api/city/id</p>
		<p>Пример: http://audiowave33.ru/api/city/5</p>
		<p>Результат:
<br>{<br>
    "id": 423,<br>
    "name": "Лянтор",<br>
    "region": "Ханты-Мансийский автономный округ",<br>
    "size": "Малый город",<br>
    "climat": "тяжелые климатические условия",<br>
    "population": "41,2 тыс.чел.",<br>
    "points": 171,<br>
    "residential and adjacent spaces": 28,<br>
    "street networks": 35,<br>
    "green spaces": 24,<br>
    "public and business infrastructure and adjacent spaces": 19,<br>
    "social and leisure infrastructure and adjacent spaces": 31,<br>
    "citywide space": 34,<br>
    "img": "https://api.индекс-городов.рф/uploads/city/emblem/3726/thumb_383_luantor.png"<br>
}</p>
	</div>
	<div>
		<h4>Случайный город</h4>
		<p><br>GET</br>http://audiowave33.ru/api/city/random</p>
		<p>Результат:<br>
{<br>
    "id": 423,<br>
    "name": "Лянтор",<br>
    "region": "Ханты-Мансийский автономный округ",<br>
    "size": "Малый город",<br>
    "climat": "тяжелые климатические условия",<br>
    "population": "41,2 тыс.чел.",<br>
    "points": 171,<br>
    "residential and adjacent spaces": 28,<br>
    "street networks": 35,<br>
    "green spaces": 24,<br>
    "public and business infrastructure and adjacent spaces": 19,<br>
    "social and leisure infrastructure and adjacent spaces": 31,<br>
    "citywide space": 34,<br>
    "img": "https://api.индекс-городов.рф/uploads/city/emblem/3726/thumb_383_luantor.png"<br>
}</p>
	</div>
	<div>
		<h4>Поиск города</h4>
		<p><br>POST</br>http://audiowave33.ru/api/city/search</p>
		<p><b>Параметры запроса:</b></p>
		<p>name - название города</p>
		<p>region - название округа или области</p>
		<p>Пример №1: http://audiowave33.ru/api/city/search<br>
			name: Тюмень</p>
		<p><br>
    {[<br>
        "id": 603,[<br>
        "name": "Тюмень",[<br>
        "region": "Тюменская область",[<br>
        "size": "Крупный город",[<br>
        "climat": "условно комфортный климат",[<br>
        "population": "807,3 тыс.чел.",[<br>
        "points": 225,[<br>
        "residential and adjacent spaces": 45,[<br>
        "street networks": 39,[<br>
        "green spaces": 35,[<br>
        "public and business infrastructure and adjacent spaces": 32,[<br>
        "social and leisure infrastructure and adjacent spaces": 41,[<br>
        "citywide space": 33,[<br>
        "img": <a href="https://api.индекс-городов.рф/uploads/city/emblem/4411/thumb_1069_Tyumen.cdr">"https://api.индекс-городов.рф/uploads/city/emblem/4411/thumb_1069_Tyumen.cdr"</a><br>
    }[<br>
</p>
		<p>Пример №2: http://audiowave33.ru/api/city/search<br>
			region: Амурская область</p>
			<p>Результат:</br>
[
    {</br>
        "id": 88,</br>
        "name": "Свободный",</br>
        "region": "Амурская область",</br>
        "size": "Средний город",</br>
        "climat": "условно комфортный климат",</br>
        "population": "54 тыс.чел.",</br>
        "points": 143,</br>
        "residential and adjacent spaces": 31,</br>
        "street networks": 27,</br>
        "green spaces": 31,</br>
        "public and business infrastructure and adjacent spaces": 12,</br>
        "social and leisure infrastructure and adjacent spaces": 22,</br>
        "citywide space": 20,</br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/4139/thumb_797_svobodniy.gif"</br>
    },</br>
    {</br>
        "id": 131,</br>
        "name": "Завитинск",</br>
        "region": "Амурская область",</br>
        "size": "Малый город",</br>
        "climat": "условно комфортный климат",</br>
        "population": "10,2 тыс.чел.",</br>
        "points": 157,</br>
        "residential and adjacent spaces": 26,</br>
        "street networks": 33,</br>
        "green spaces": 28,</br>
        "public and business infrastructure and adjacent spaces": 20,</br>
        "social and leisure infrastructure and adjacent spaces": 23,</br>
        "citywide space": 27,</br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/3548/thumb_203_Zavitinsk.PNG"</br>
    },</br>
    {</br>
        "id": 191,</br>
        "name": "Райчихинск",</br>
        "region": "Амурская область",</br>
        "size": "Малый город",</br>
        "climat": "условно комфортный климат",</br>
        "population": "16,8 тыс.чел.",</br>
        "points": 172,</br>
        "residential and adjacent spaces": 30,</br>
        "street networks": 28,</br>
        "green spaces": 34,</br>
        "public and business infrastructure and adjacent spaces": 23,</br>
        "social and leisure infrastructure and adjacent spaces": 30,</br>
        "citywide space": 27,</br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/3899/thumb_556_Raychikhinsk.gif"</br>
    },</br>
    {</br>
        "id": 371,</br>
        "name": "Белогорск",</br>
        "region": "Амурская область",</br>
        "size": "Средний город",</br>
        "climat": "условно комфортный климат",</br>
        "population": "65,3 тыс.чел.",</br>
        "points": 162,</br>
        "residential and adjacent spaces": 29,</br>
        "street networks": 28,</br>
        "green spaces": 30,</br>
        "public and business infrastructure and adjacent spaces": 16,</br>
        "social and leisure infrastructure and adjacent spaces": 28,</br>
        "citywide space": 31,</br>
        "img": "https://api.индекс-городов.рф/uploads/city/emblem/4202/thumb_860_Belogorsk.png"</br>
    },...</br>
    И так далее</p>
	</div>
