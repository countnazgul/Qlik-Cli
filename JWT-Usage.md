**Obtain your JWT to accessing Qlik Sense first!**

* create new file in your user home folder (`C:\Users\My-UserName`)
* name the file `.qlik-cli`
* the file is in JSON format and will contain all of your tokens for the different Qlik Sense instances:

```json
{
    "dev": "my-long-token-for-accessing-DEV",
    "test": "my-long-token-for-accessing-TEST",
    "prod": "my-long-token-for-accessing-PROD",
    ...
}
```

* when starting `Qlik-Cli` specify the `-Token` parameter and the environment name:

```
Connect-Qlik -computerName qlik-sense-proxy/jwt-vp -Token dev
```

**Make sure that the correct Virtual Proxy is specified and that the VP is set to authenticate with JWT**