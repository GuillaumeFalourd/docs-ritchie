---
title: Use credentials as formula inputs
weight: 61
description: In this section, you will find how to set credentials as inputs.
---

---

Once a provider's credential has been set, it can be used as input in the formula's **`config.json`**file. To do so, it is necessary to use the reserved keyword:**`CREDENTIAL`**

When used as an input, the credential will contain 2 fields:

* The **name** is the variable used to extract the input and manipulate it inside the formula's code.
* The **type** is the specific nomenclature for the CLI to now which credential to use.

{{% alert color="danger" %}}
The **type** needs to respect the following pattern: **`CREDENTIAL_PROVIDER_VARIABLE`**
{{% /alert %}}

For example, to be able to use **`GITHUB`** credentials as input, you need to inform them as follows in the formula's **`config.json`** file:

```text
"inputs": [ 
    { 
        "name": "git_user", 
        "type": "CREDENTIAL_GITHUB_USERNAME" 
    },
    { 
        "name": "git_email", 
        "type": "CREDENTIAL_GITHUB_EMAIL" 
    },
    { 
        "name": "git_token", 
        "type": "CREDENTIAL_GITHUB_TOKEN"
    } 
]
```

If you have any doubt regarding the provider's variable names, you can check the credentials you've set using the following command:

```text
rit list credential
```

With **`GITHUB`**, it will return something like this:

```text
PROVIDER	 CONTEXT	  CREDENTIAL
github  	 default	  {"token":"***", "email":"***", "username":"***"}
```

## Next steps 

You saw in this section how to deal with credentials on Ritchie. 

👉 Check the [**commands list**]({{< ref path="Reference/List of commands and flags.md" >}}) to see the available automations on our community repo.
