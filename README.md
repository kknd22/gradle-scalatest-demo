# gradle-scalatest-demo
gradle scalatest demo to show issue with org.apache.cxf:cxf-rt-frontend-jaxws:3.1.5

`./gradlew test`   
```
An exception or error caused a run to abort. This may have been caused by a problematic custom reporter.
java.lang.IncompatibleClassChangeError: Implementing class
	at java.lang.ClassLoader.defineClass1(Native Method)   
```

```
// -- comment out the following line will make the test sucessful
    compile 'org.apache.cxf:cxf-rt-frontend-jaxws:3.1.5'
```
