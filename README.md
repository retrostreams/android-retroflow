# android-retroflow

android-retroflow is a backport of the new Java 9 (JEP 266) reactive-streams Flow and SubmissionPublisher API for Android developers wanting to use the Android Studio 3.0 desugar toolchain.

There is nothing specific to Android or the desugar toolchain in this code (it could even be compiled to Java 6 bytecode) but
it has a dependency on [android-retrostreams](https://github.com/retrostreams/android-retrostreams) which is why this exists as a separate component (the corresponding
[streamsupport-flow](https://sourceforge.net/p/streamsupport/code/ci/default/tree/src/flow/) component can't be used with android-retrostreams).


## LICENSE

GNU General Public License, version 2, with the Classpath Exception
