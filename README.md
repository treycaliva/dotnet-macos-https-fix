# dotnet-macos-https-fix

FYI, if you're running into an issue getting dotnet to serve your project (specifically if the browser is complaining about a secure connection or Chorme shows an "ERR_SSL_PROTOCOL_ERROR") the following commands should help you out.

```bash
dotnet dev-certs https
dotnet dev-certs https --trust
```

[Referenced GitHub issue from dotnet/runtime](https://github.com/dotnet/runtime/issues/27132)
