# AndroidHelper - GitHub Copilot Custom Agent

A simple GitHub Copilot custom agent for Android development in Kotlin.

## Description

This custom agent helps with common Android development tasks using simple commands.

## Available Commands

### `/cleanup`
Cleans up and optimizes import statements in Kotlin files.

**Usage:** Select Kotlin code and run `@AndroidHelper /cleanup`

### `/viewmodel`
Generates a ViewModel class for your Activity following MVVM architecture pattern.

**Usage:** In your Activity file, run `@AndroidHelper /viewmodel`

### `/test`
Generates comprehensive unit tests for selected Kotlin functions.

**Usage:** Select a function and run `@AndroidHelper /test`

### `/binding`
Converts Activity or Fragment to use ViewBinding.

**Usage:** In your Activity/Fragment file, run `@AndroidHelper /binding`

## Installation

1. Enable GitHub Copilot Extensions in your GitHub account
2. Connect this repository as a custom Copilot agent
3. Use the agent in Android Studio with `@AndroidHelper` followed by a command

## Requirements

- GitHub Copilot subscription
- Android Studio
- GitHub Copilot Extensions enabled

## Example

```kotlin
// In MainActivity.kt, type:
@AndroidHelper /viewmodel

// The agent will generate a ViewModel like:
class MainViewModel : ViewModel() {
    private val _data = MutableLiveData<String>()
    val data: LiveData<String> = _data
    
    // Your logic here
}
```

## License

MIT
