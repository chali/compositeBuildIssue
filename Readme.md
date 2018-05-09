# Example for dependencies output difference

    cd consumer
    ./gradlew dependencies --configuration compile

Gradle 4.7:

    compile - Dependencies for source set 'main' (deprecated, use 'implementation ' instead).
    \--- example:b:1.0.0 -> project :included-project:b
        \--- project :included-project:a

Gradle 4.8 nightly:
 
    compile - Dependencies for source set 'main' (deprecated, use 'implementation ' instead).
    \--- example:b:1.0.0 -> project :included-project:b
        \--- project :included:a