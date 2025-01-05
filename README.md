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
|26|1.14|https://github.com/alzo-archi/jinterface-build/releases/download/v1.14-otp26-java21/OtpErlang-otp26-java21-1.14.jar|39baf7294bdde946d5335a7bb0221194ddab986c76813cbaa15e5113c7934848|
|25|1.13.2|https://github.com/alzo-archi/jinterface-build/releases/download/v1.13.2-otp25-java21/OtpErlang-otp25-java21-1.13.2.jar|deecea6dba2d2a72f830355bc25f9486ec03d3e1e896bc6c95babb5783510d2e|
