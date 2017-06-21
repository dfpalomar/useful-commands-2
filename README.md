# useful-commands-2

* Check Java installation path on Mac OS X

```(/usr/libexec/java_home)```

* Download a server public certificate

```echo -n | openssl s_client {HOST}:{PORT(443)} | sed -ne '/-BEGIN CERTIFICATE-/,/-END CERTIFICATE-/p' > ./{CERT_FILE_NAME}.crt```

* How to stop Gradle task execution in Android Studio?

```./gradlew --stop```

* Print project dependencies as ascii tree

```./gradlew dependencies```

* Print project dependencies as ascii tree for a multi-module project. Add the following to the root build.gradle file and then run the task

```
subprojects {
    task allDeps(type: DependencyReportTask) {}
}
```

* Guide to install SSH key and adding it to the SSH agent

https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/

* Add certificate to the Java keystore

```sudo keytool -import -trustcacerts -alias example.com -file ./the_website_cert.pem -keystore $JAVA_HOME/jre/lib/security/cacerts```

* Cron job online generator

```https://crontab.guru/every-month```
