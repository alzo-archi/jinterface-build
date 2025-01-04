# Jinterface-build

Action that builds the Jinterface / OtpErlang jar file for OTP 27, OTP 26, OTP 25, with JDK 21, since the Jinterface version on Maven is more than outdated.

See the RELEASES to get the build corresponding to your OTP version.
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
