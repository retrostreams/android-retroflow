[![Maven Central](https://img.shields.io/maven-central/v/net.sourceforge.streamsupport/android-retroflow.svg)](http://mvnrepository.com/artifact/net.sourceforge.streamsupport/android-retroflow)
[![javadoc.io](https://javadocio-badges.herokuapp.com/net.sourceforge.streamsupport/android-retroflow/badge.svg)](http://www.javadoc.io/doc/net.sourceforge.streamsupport/android-retroflow/)
[![Download](https://api.bintray.com/packages/stefan-zobel/android-retroflow/android-retroflow/images/download.svg) ](https://bintray.com/stefan-zobel/android-retroflow/android-retroflow/_latestVersion)

# android-retroflow

![](art/streamsupport-sf.png)

android-retroflow is a backport of the new Java 9 (JEP 266) reactive-streams Flow and SubmissionPublisher API for Android developers wanting to use the Android Studio 3.0 desugar toolchain.

There is nothing specific to Android or the desugar toolchain in this code (it could even be compiled to Java 6 bytecode) but
it has an indirect dependency on [android-retrostreams](https://github.com/retrostreams/android-retrostreams) (via [android-retrofuture](https://github.com/retrostreams/android-retrofuture)) which is why this exists as a separate component (the corresponding
[streamsupport-flow](https://github.com/stefan-zobel/streamsupport/tree/master/src/flow) component can't be used with android-retrostreams
and [android-retrostreams](https://github.com/retrostreams/android-retrostreams) itself can *only* be used with desugar or Java 8 / 9).

Other than having a different package name this code has no further changes compared with [streamsupport-flow](https://github.com/stefan-zobel/streamsupport/tree/master/src/flow)

Online Javadoc is available at [docs](https://retrostreams.github.io/android-retroflow/apidocs/index.html)

Please give feedback [here](https://github.com/retrostreams/android-retroflow/issues) if you experience any problems.


### build.gradle:

```gradle
dependencies {
    compile 'net.sourceforge.streamsupport:android-retroflow:1.6.2'
}
```

## LICENSE

GNU General Public License, version 2, with the Classpath Exception
