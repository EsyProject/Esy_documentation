import BoxMethod from '/src/components/MethodBox/BoxMethod.jsx';

# Assessment 🌟

Seu feedback é valioso para nós! Queremos garantir que cada evento seja uma experiência incrível para todos os participantes. Por favor, dedique alguns minutos para nos fornecer sua opinião sobre o evento que você acabou de participar.

## Endpoints Assessment:

BaseUrl: `http://172.28.69.4:6968/assessment`

### Register Assessment:

<BoxMethod
    method='POST'
    endpoint='/assessment/{event_id}'
/>

> Type: `JSON`

**Attributes:**
```
suggestion: String
description_comment: String
highlightPoint: String
assessment: Integer
```

**Return:**

Statos code: `201 created`

~~~json
{
	"assessment_id": "Long",
	"author": "String",
	"suggestion": "String",
	"description_comment": "String",
	"assessment": "Integer",
	"hour": "LocalTime",
	"date_created": "LocalDate",
	"highlightPoint": "String"
}
~~~


### Pegar assessments:

**GET assessment based in Event ID:**

<BoxMethod
    method='GET'
    endpoint='/assessment/assessments/{event_id}'
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
	"imgUrl": "List<String> Url",
	"localEvent": "String",
	"initialDate": "Date",
	"finishDate": "Date",
	"initialTime": "Time",
	"finishTime": "Time",
	"assessments": "List<Assessment>"
}
~~~

**Assessment return:**

~~~json
{
	"assessment_id": "Long",
	"date_created": "Local Date",
	"hour": "Local Time",
	"author": "String",
	"description_comment": "String",
	"suggestion": "String",
	"highlightPoint": "String",
	"assessment": "Integer"
}
~~~