import BoxMethod from '/src/components/MethodBox/BoxMethod.jsx';

# Ticket 🎟

Bem-vindo à nossa plataforma de tickets de suporte! Aqui você pode criar, acompanhar e resolver problemas ou solicitações de suporte de maneira eficiente e organizada. Nossa equipe está aqui para ajudá-lo a resolver qualquer problema que você possa enfrentar.

## Endpoints Ticket:

BaseUrl: `http://172.28.69.4:6968/ticket`

### Register Ticket:

<BoxMethod
    method='POST'
    endpoint='/ticket'
/>

> Type: `JSON`

**Attributes:**

```
initialDateTicket: Date,
finishDateTicket: Date,
initialTimeTicket: Time,
finishTimeTicket: Time
```

**Return:** 

Status code: `201 created`

~~~json
{
{
	"ticket_id": "Long",
	"initialDate": "Date",
	"finishDate": "Date",
	"initialTime": "Time",
	"finishTime": "Time",
	"date_created": "LocalDate",
	"timeCreated": "LocalTime",
	"qrCodeNumber": "Integer"
}
}
~~~