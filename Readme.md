# Example for dependencies output difference

    cd can-use-recommender-in-a-composite
    ./gradlew dependencies --configuration compile

Gradle 4.7:

    compile - Dependencies for source set 'main' (deprecated, use 'implementation ' instead).
    \--- example:b:1.0.0 -> project :can-use-recommender-in-a-composite:b
        \--- project :can-use-recommender-in-a-composite:a

Gradle 4.8 nightly:
 
    compile - Dependencies for source set 'main' (deprecated, use 'implementation ' instead).
    \--- example:b:1.0.0 -> project :can-use-recommender-in-a-composite:b
        \--- project :can-use-recommender-in-a-composite-composite:a