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
                "Jetpack, View/Data Binding, Fragments, RecyclerView, Room, " +
				"Retrofit, LiveData, RxJava3, Dagger2, Coroutines, " +
				"BroadcastReceivers, ContentProviders",
        "Backend" to "Flask, SQLite, SqlAlchemy, Firebase (Realtime database, Auth)",
        "GameDev" to "UnityEngine, Pygame"
    )

    val architecturePatterns = listOf(
        "MVVM", "Clean Architecture, Dependency Injection"
    )

    fun getStudiedNow(): Technology {
        return Kotlin.Coroutines.Flow
    }

    fun sayHello() {
        println("Hello! Welcome at my Github Profile!")
    }
}
