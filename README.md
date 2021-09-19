[![Maven Central](https://img.shields.io/maven-central/v/net.sourceforge.streamsupport/android-retroflow.svg)](http://mvnrepository.com/artifact/net.sourceforge.streamsupport/android-retroflow)
[![javadoc.io](https://javadoc.io/badge2/net.sourceforge.streamsupport/android-retroflow/javadoc.svg)](https://javadoc.io/doc/net.sourceforge.streamsupport/android-retroflow)

# android-retroflow

![](art/streamsupport-sf.png)

android-retroflow is a backport of the new Java 9 (JEP 266) reactive-streams Flow and SubmissionPublisher API for Android developers wanting to use the Android Studio 3.x D8 / desugar toolchain.

There is nothing specific to Android or the desugar toolchain in this code (it could even be compiled to Java 6 bytecode) but
it has an indirect dependency on [android-retrostreams](https://github.com/retrostreams/android-retrostreams) (via [android-retrofuture](https://github.com/retrostreams/android-retrofuture)) which is why this exists as a separate component (the corresponding
[streamsupport-flow](https://github.com/stefan-zobel/streamsupport/tree/master/src/flow) component can't be used with android-retrostreams
and [android-retrostreams](https://github.com/retrostreams/android-retrostreams) itself can *only* be used with desugar or Java 8 and higher).

Other than having a different package name this code has no further changes compared with [streamsupport-flow](https://github.com/stefan-zobel/streamsupport/tree/master/src/flow)

Online Javadoc is available at [docs](https://retrostreams.github.io/android-retroflow/apidocs/index.html)

Please give feedback [here](https://github.com/retrostreams/android-retroflow/issues) if you experience any problems.


### build.gradle:

```gradle
dependencies {
    implementation 'net.sourceforge.streamsupport:android-retroflow:1.7.4'
}
```

## LICENSE

GNU General Public License, version 2, [with the Classpath Exception](https://github.com/retrostreams/android-retroflow/blob/master/GPL_ClasspathException)  (and [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) for JSR-166 derived code)
