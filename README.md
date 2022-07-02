
# Take Blip - API Notificações

Código fonte em python criado por **Pedro Lucas**: https://github.com/ZumbiDoPython

Função em Lambda / API Gateway convertida por **Breno Andrade**: https://github.com/brenooandrade

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)


## Documentação da API

#### Envia de notificações

```http
  POST /prod/send_notification
```

| Header   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `x-api-key` | `string` | **Obrigatório**. Chave de segurança API Gateway |
| `Authorization` | `string` | **Obrigatório**. Authorization Take Blip |
| `namespace` | `string` | **Obrigatório**. namespace Take Blip |

#### Modelo de Payload (JSON Body)

```http
{
    "phone": "11 9XXXXX86",
    "name": "Breno Andrade",
    "template": "nps_2022v1",
    "state_id": "17402715-0cd2-4c7c-a279-4d2d93a9f9", 
    "flow_id": "3da8f490-7a24-43c2-b83e-36a15e2774",
    "id_bot": "clienteprincipal",
    "extras": {"Teste":"Mensagem para o cliente"},
    "content":[]
}
```


