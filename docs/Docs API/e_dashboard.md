import BoxMethod from '/src/components/MethodBox/BoxMethod.jsx';

# Dashboard 🎯

Bem-vindo ao nosso Dashboard! Aqui você encontrará uma visão geral das principais métricas e informações relevantes para o seu negócio. Este painel foi projetado para oferecer insights claros e acionáveis para ajudá-lo a tomar decisões informadas.


## Endpoints Dashboard:

BaseUrl: `http://172.28.69.4:6968/dashboard`

### Pegar Dados Eventos (Dashboard):

**GET Average Of Event:**

<BoxMethod
    method='GET'
    endpoint='/dashboard/average/{event_id}'
/>


**Return:**

Statos code: `200 OK`

~~~json
{
	"average": "Integer"
}
~~~

**GET HighPointsGraph:**

<BoxMethod
    method='GET'
    endpoint='/dashboard/highPoints/{event_id}'
/>


**Return:**

Statos code: `200 OK`

~~~json
{
	"event_id": "Long",
	"food": "Integer",
	"topics_addressed": "Integer",
	"punctuality": "Integer",
	"social_interactions": "Integer"
}
~~~


**GET Suggestions based in Assessment:**

<BoxMethod
    method='GET'
    endpoint='/dashboard/suggestion/{event_id}'
/>


**Return:**

Statos code: `200 OK`

~~~json
[
	{
		"id": "Long",
		"date_suggestion": "Date",
		"message_suggestion": "String"
	}
]
~~~
