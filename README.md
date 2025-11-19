# CoreIcons Module

This module provides centralized access to all drawable icons in the core module.

## Usage

To use an icon from this module, call the `getIcons` function with one of the constants from `GetIcons.Icon`.

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
