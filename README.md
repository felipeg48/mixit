# Mix-IT 2017 website

To run the application:
```
./gradlew bootRun
```

To package and run the application from the executable JAR:
```
./gradlew build
cd build/libs/
java -jar mixit-1.0.0-SNAPSHOT.jar
```

To enable live reload of static resources:
```
./gradlew processResources -t
```

To test the application from a browser:
```
http://localhost:8080/index.html
http://localhost:8080/user/1
```


## Installation

### KAPT

Persistent entities interfaces are enhanced with code generation using KAPT (Annotation Processing for Kotlin)

To enable IntelliJ IDEA syntax highlight you must add the sources generated by KAPT to the indexed contents: 
  ```
  File -> Project structure -> modules -> mixit_main -> Add content root : "build/generated/source/kapt"
```