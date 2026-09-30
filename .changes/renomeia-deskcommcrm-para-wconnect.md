---
impacto: nada_mudou
secao: alterado
titulo: O produto agora se chama WConnect — o nome trocou no instalador, nas mensagens e nos guias
---

O nome antigo saiu de tudo o que a pessoa lê: as telas e as mensagens do instalador, os erros do kit, o README e os guias agora falam em WConnect, o repositório passou a ser `Masukulmiguel/wconnect` e o clone novo por padrão é a pasta `wconnect`.

Quem já tem o CRM numa VPS não precisa fazer nada para atualizar. O diretório da instalação, o nome do projeto dos contêineres e as variáveis do `.env` continuam os mesmos — eles vêm do que está no disco, não do default novo — e o `update.sh` de sempre atualiza o que já está no ar.

Só dois nomes trocaram de verdade, e nenhum dos dois trava a atualização: o marcador de instalação virou `.wconnect-instalado` (o `update.sh` grava o novo ao terminar, ao lado do antigo) e a saída de emergência para duas cópias do repo disputando os mesmos contêineres passou de `DESKCOMM_ASSUMIR_PROJETO` para `WCONNECT_ASSUMIR_PROJETO`. Quem tinha o nome antigo escrito no crontab troca quando for usar de novo.
