# CoreIcons Module [![](https://jitpack.io/v/zeesofttechlibraries/Core-Icons.svg)](https://jitpack.io/#zeesofttechlibraries/Core-Icons)

This module provides centralized access to all drawable icons in the core module.

## Dependency

First, add the JitPack repository to your `settings.gradle` or `settings.gradle.kts` file:

```kotlin
// settings.gradle.kts
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        mavenCentral()
        maven { url = uri("https://jitpack.io") }
    }
}
```

Next, add the following dependency to your `build.gradle` or `build.gradle.kts` file:


```kotlin
// build.gradle.kts
dependencies {
    implementation("com.github.zeesofttechlibraries:Core-Icons:1.0.0")
}
```

## Usage

To use an icon from this module, first import `GetIcons`:

```kotlin
import com.zeesofttechlibraries.coreicons.GetIcons
```

Then, call the `getIcons` function with one of the constants from `GetIcons.Icon`.

```kotlin
val iconId = GetIcons.getIcons(GetIcons.Icon.BACK_IC)
imageView.setImageResource(iconId)
```

The `getIcons` function returns the drawable resource ID for the given icon name.

### Available Icons

You can find the list of all available icon constants inside the `GetIcons.Icon` sealed interface. The IDE will provide autocomplete and hover hints for all available icon names.

### Benefits

1.  **Clean Drawable Folders**: Keeps the drawable folders in feature modules clean.
2.  **Reusability**: Reuse icons across the app without duplicating resources.
3.  **IDE Friendly**: Autocomplete and hover hints in the IDE show all available icon names, making it easy to find the icon you need.
