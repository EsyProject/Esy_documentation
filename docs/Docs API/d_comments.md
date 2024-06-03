import BoxMethod from '/src/components/MethodBox/BoxMethod.jsx';

# Comments 📋

Seus comentários são importantes para nós! Queremos garantir que cada interação com nossos serviços seja positiva e produtiva. Por favor, compartilhe suas opiniões e sugestões conosco para que possamos continuar a melhorar.

* Comentário é baseado nos endpoints de avaliação (Assessment)

## Endpoint Comment:

BaseUrl: `http://172.28.69.4:6968/assessment`

### Pegar Comentário:

<BoxMethod
    method='GET'
    endpoint='/assessment/comments/{event_id}'
/>


**Return:**

Statos code: `200 OK`

~~~json
[
	{
		"comment_id": "Long",
		"author": "String",
		"description_comment": "String",
		"date_created": "Date",
		"assessment": "Integer"
	}
]
~~~