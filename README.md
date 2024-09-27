# EcomAndroidSdkPackages

Артефакты Android сборки EcomSdk

Подключение:

Добавить мавен в ```settings.gradle```
```
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven {
            name = "GitHubPackages"
            url = uri("https://maven.pkg.github.com/sdkpay/EcomAndroidSdkPackages")
        }
    }
}
```
Добавить зависимость в ```build.gradle```
```
implementation("ru.spaymentsplus.libraries-debug:ecomsdk:$version")
```
