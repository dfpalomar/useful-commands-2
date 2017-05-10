# useful-commands-2

* Check Java installation path on Mac OS X

```(/usr/libexec/java_home)```

* Download a server public certificate

```echo -n | openssl s_client {HOST}:{PORT(443)} | sed -ne '/-BEGIN CERTIFICATE-/,/-END CERTIFICATE-/p' > ./{CERT_FILE_NAME}.crt```


