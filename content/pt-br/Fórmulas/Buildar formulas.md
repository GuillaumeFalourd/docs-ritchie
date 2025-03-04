---
title: Buildar fórmulas
weight: 42
description: Nesta seção, você encontrará o passo a passo para fazer o build de fórmulas no Ritchie.
---

---

{{% alert color="danger" %}}

Essa funcionalidade não está mais disponível a partir da **versão 2.5.0 do Ritchie.** Isso porque o build da fórmula é feito de maneira automática: um repositório local criado assim que você implementa a fórmula
Caso esteja usando uma versão anterior, basta seguir as orientações desta seção. 


{{% /alert %}}

## Como "buildar"?

Depois de [**criar uma formula**]({{< ref path="/Fórmulas/Criar fórmulas.md" >}}), e se você quiser editar o código dela, será necessário fazer o build dessas alterações para testar o comando com a nova implementação. 

Para isso, basta executar o comando:  

```text
rit build formula
```

Você deverá informar: 

* O caminho  do diretório onde a fórmula está localizada.
* O caminho da fórmula a ser buildada (ele segue o comando da fórmula). 

Caso queira atualizar o código da fórmula em tempo de execução, é possível utilizar a **flag “--watch”** junto da fórmula. Veja no exemplo abaixo:

```text
rit build formula --watch
```
