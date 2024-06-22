```kotlin
package com.kaelesty.personal_info

class GithubProfile(): InternetProfile() {

    val education = mapOf(
        "Yandex Lyceum" to TimePeriod(start=2019, end=2021),
        "Saint-Petersburg State University of Aerospace Instrumentation" to TimePeriod(start=2022, isInProgress=true)
    )

    val programmingLanguages = listOf(
        Kotlin::class, Python::class, Java::class, CSharp::class, Cpp::class // Descending by skills
    )

    val technologyStack = mapOf(
        "Android Development" to
                "Jetpack Compose, Jetpack Navigation, Decompose, MVIKotlin, Room, " +
				"Retrofit, Dagger, Coroutines",
        "Backend" to "Ktor, Exposed, Flask, SqlAlchemy, Firebase",
        "GameDev" to "UnityEngine, Pygame"
    )

    val architecturePatterns = listOf(
        "MVVM", "MVI", "Clean Architecture", "Dependency Injection"
    )

    fun getStudiedNow(): List<Learnable> {
        return listOf( Kotlin.Multiplatform, Backend.Ktor, ComputerScience.Algorithms,  ComputerScience.DataStructures )
    }

    fun sayHello() {
        println("Hello! Welcome at my Github Profile!")
    }
}
