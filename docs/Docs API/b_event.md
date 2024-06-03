import BoxMethod from '/src/components/MethodBox/BoxMethod.jsx';

# Event 🎉

Junte-se a nós para uma experiência única e memorável no nosso evento especial! Na plataforma EsyBosch, você pode criar e personalizar seu próprio evento de forma fácil e rápida. Adicione fotos incríveis, uma descrição envolvente e todos os detalhes importantes, como data, local, entre outros.

## Endpoints Event:

BaseUrl: `http://172.28.69.4:6968/event`

### Register Event:

<BoxMethod
    method='POST'
    endpoint='/event'
/>

> Type: `Multipartform`

**Attributes:**

```
nameOfEvent: String
responsivle_area: String
access_event: String
description: String
images: file (Optional)
localEvent: String
initialDate: Date
finishDate: Date
initialTime: Time
finishTime: Time
```

**Return:** 

Status code: `201 created`

~~~json
{
	"event_id": "Long",
	"nameOfEvent": "String",
	"responsible_area": "String",
	"access_event": "String",
	"description": "String",
	"imgUrl": "List<String> url",
	"localEvent": "String",
	"initialDate": "Date",
	"finishDate": "Date",
	"initialTime": "Time",
	"finishTime": "Time",
	"date_created": "LocalDate",
	"time_created": "LocalTime",
	"author": "String"
}
~~~

### Pegar eventos:

**GET All Events:**

<BoxMethod
    method='GET'
    endpoint='/event/events'
/>

**Return:** 

Status code: `200 OK`

~~~json
[
    {
		"event_id": "Long",
		"nameOfEvent": "String",
		"responsible_area": "String",
		"access_event": "String",
		"description": "String",
		"localEvent": "String",
		"initialDate": "Date",
		"finishDate": "Date",
		"initialTime": "Time",
		"finishTime":"Time",
		"imgUrl": "List<String> url"
	}
]
~~~



**GET Find by ID:**

<BoxMethod
    method='GET'
    endpoint='/event/{event_id}'
/>

**Return:** 

Status code: `200 OK`

~~~json
{
	"event_id": "Long",
	"nameOfEvent": "String",
	"responsible_area": "String",
	"access_event": "String",
	"description": "String",
	"imgUrl": "List<String> url",
	"localEvent": "String",
	"initialDate": "Date",
	"finishDate": "Date",
	"initialTime": "Time",
	"finishTime": "Time",
	"date_created": "LocalDate",
	"time_created": "LocalTime",
	"author": "String"
}
~~~


**GET Event name:**

<BoxMethod
    method='GET'
    endpoint='/event/name'
/>

**Return:** 

Status code: `200 OK`

~~~json
{
	"event_id": "Long",
	"nameOfEvent": "String"
}
~~~


**GET My events:**

<BoxMethod
    method='GET'
    endpoint='/event/myEvent'
/>

**Return:** 

Status code: `200 OK`

~~~json
{
	"event_id": "Long",
	"nameOfEvent": "String",
	"initialDate": "Date",
	"initialTime": "Time",
	"local": "String",
	"responsible_are": "String"
}
~~~


**GET Event Feed:**

<BoxMethod
    method='GET'
    endpoint='/event/feed'
/>

**Return:** 

Status code: `200 OK`

~~~json
{
	"event_id": "Long",
	"nameOfEvent": "String",
	"initialDate": "Date",
	"initialTime": "Time",
	"finishTime": "Time",
	"description": "String",
	"local": "Time",
	"responsible_area": "String",
	"imgUrl": "List<String> Url"
}
~~~

**GET Card Event:**

<BoxMethod
    method='GET'
    endpoint='/event/card'
/>

**Return:** 

Status code: `200 OK`

~~~json
{
	"event_id": "Long",
	"initialDate": "Date",
	"nameOfEvent": "String",
	"description": "String"
}
~~~

