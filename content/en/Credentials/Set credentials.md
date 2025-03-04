---
title: Set credentials
weight: 55
description: In this section, you will find how to set credentials.
---

---

You have to set Ritchie's credentials to avoid informing data multiples times through the terminal.

To do so, just run the following command: 

```text
rit set credential
```

The terminal will return this message: 

```text
? Select your provider  [Use arrows to move, type to filter]
> kubeconfig
  ansible
  aws
  github
  gitlab
  jenkins
  Add a new
```

After you chose one of the available providers, Ritchie will ask you to fill the following fields: 

```text
? Select your provider github
? username: DennisRitchie
? email: dennis.ritchie@zup.com.br
? token: 
✔ Github credential saved!
```

{{% alert color="info" %}}
You can check out on [**formula's editable files**]({{< ref path="/Formulas/Organize the Formula Folder.md" >}}) to see how to manipulate the credentials defined in the session as formula input parameters \(inputs in the config.json file\).
{{% /alert %}}
