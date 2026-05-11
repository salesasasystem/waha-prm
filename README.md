# WAHA PRM

Servidor WAHA para o PRM consultar membros reais de grupos do WhatsApp.

Este deploy usa o engine `GOWS`, que evita abrir navegador/Chromium no Render e tende a iniciar melhor em plano gratuito.

## Variaveis no Render

Configure no painel do Render:

```txt
WAHA_API_KEY=coloque-uma-chave-grande
WAHA_DASHBOARD_USERNAME=admin
WAHA_DASHBOARD_PASSWORD=coloque-uma-senha-grande
WHATSAPP_DEFAULT_ENGINE=GOWS
```

Depois do deploy, abra:

```txt
https://SEU-SERVICO.onrender.com/dashboard
```

Faça login no dashboard, inicie a sessao `default` e leia o QR Code com o WhatsApp.

## Teste rapido

Troque a URL e a chave:

```bash
curl -H "X-Api-Key: SUA_CHAVE" \
  "https://SEU-SERVICO.onrender.com/api/default/groups/5511986100004-1603680717%40g.us/participants/v2"
```
