# Jinterface-build

Action that builds the Jinterface / OtpErlang jar file for OTP 27, OTP 26, OTP 25, with JDK 21, since the Jinterface version on Maven is more than outdated.

See the [RELEASES](https://github.com/alzo-archi/jinterface-build/releases) to get the build corresponding to your OTP version.
Use it in your Java project with :

```sh
mvn install:install-file \
    -Dfile=./OtpErlang-VERSION.jar \
    -DgroupId=org.ericsson.otp \
    -DartifactId=jinterface \
    -Dversion=VERSION \
    -Dpackaging=jar \
    -DgeneratePom=true
```

|OTP Version|Jinterface Version|URL|SHA256|
|---|---|---|---|
|27|1.14.1|https://github.com/alzo-archi/jinterface-build/releases/download/v1.14.1-otp27-java21/OtpErlang-otp27-java21-1.14.1.jar|cab039f7cb7b1458c227534403fa3b7309945c154380e671ddb16e2b8268a85b|
