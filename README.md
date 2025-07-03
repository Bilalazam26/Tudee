#  Tudee – Jetpack Compose Task MAnagement App

As a Team, our task is to develop a personal task management app for Android.

---

## 📦 Download Tudee APK

You can download and install the latest version of Tudee here:

[⬇️ Download Tudee APK (v1.0.0)](https://github.com/Bilalazam26/Tudee/releases/download/v1.0.0/Cute_Tudee.apk)

---

## 📸 Screen Shots
<table>
  <tr>
    <td align="center">
      <strong>Splash Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/46943ce5-cc19-45fd-b1ea-a9d5744f7ece" width="200"/>
    </td>
    <td align="center">
      <strong>Onboarding Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/30f3a9b7-57fa-41f0-8bd8-4be9acec797d" width="200"/>
    </td>
    <td align="center">
      <strong>Onboarding Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/fa3a924b-33cd-45f4-9ca7-1ff0b09e5ae7" width="200"/>
    </td>
    <td align="center">
      <strong>Home Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/58eeced0-4982-4a98-b216-d1b679af5cb8" width="200"/>
    </td>
  </tr>

  <tr>
    <td align="center">
      <strong>Home Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/d78669b0-3882-4d45-8ee5-8100ff0be627" width="200"/>
    </td>
    <td align="center">
      <strong>Task Details Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/b0f4401c-bc30-4884-a6c7-bdd053eb6713" width="200"/>
    </td>
    <td align="center">
      <strong>Tasks Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/7fb7969f-0d84-4206-8996-8c151336a1c7" width="200"/>
    </td>
    <td align="center">
      <strong>Categories Screen Dark</strong><br/>
      <img src="https://github.com/user-attachments/assets/74edc22c-5b7c-4374-83cf-044691047013" width="200"/>
    </td>
  </tr>

<tr>
  <td align="center">
      <strong>Home Screen Light</strong><br/>
      <img src="https://github.com/user-attachments/assets/abb9a0c9-327c-479a-ac11-ab532898573c" width="200"/>
    </td>
  <td align="center">
      <strong>Task Details Light</strong><br/>
      <img src="https://github.com/user-attachments/assets/ee9500ab-0a94-48d8-9849-53ee0866a7dd" width="200"/>
    </td>
    <td align="center">
      <strong>Delete Task Light</strong><br/>
      <img src="https://github.com/user-attachments/assets/bec8cda0-8b4e-4533-9b40-afb689bcfa99" width="200"/>
    </td>
    <td align="center">
      <strong>Add Task Light</strong><br/>
      <img src="https://github.com/user-attachments/assets/82c56457-a8b5-4bef-aef5-c3996cc29aff" width="200"/>
    </td>
  </tr> 
</table>

---

## 📸 Theme Toggling Quick Demo

<p align="left">
  
https://github.com/user-attachments/assets/7a1de2cf-72bc-42a8-a621-11d3e5a0ed73

</p>

---

## 🧠 Key Concepts

This app is a practical demonstration of:

- Jetpack Compose UI
- Clean MVI Architecture
- Koin for Dependency Injection
- Coil
- Single Responsibility & SOLID Principles

---

## 📱 Features

- onboarding screen to appear only the first time I launch the app.
- home screen displaying statistics about today’s tasks.
- create a new task with a title, description, priority, and category.
- view the full details of any task.
- view all tasks based on a selected date.
- delete any task.
- change a task’s status from "To Do" to "In Progress," and from "In Progress" to "Done."
- see a list of predefined categories.
- add a new category, including selecting an image from my device.
- edit or delete any category that I created.
- switch between light and dark mode.
- the app to follow the device’s language settings and support both English and Arabic (no separate settings screen is required).

---

## 🛠️ Tech Stack

| Tech                    | Usage                         |
|-------------------------|-------------------------------|
| **Kotlin**              | Programming Language          |
| **Jetpack Compose**     | Declarative UI Framework      |
| **MVI**                 | Architecture Pattern          |
| **Koin**                | Dependency Injection          |

---
## 🧩 Architecture
<pre>
├── data
│   ├── database
│   │   ├── CategoryDao.kt
│   │   ├── TaskDao.kt
│   │   └── TudeeDatabase.kt
│   ├── mapper
│   │   ├── CategoryMapper.kt
│   │   └── TaskMapper.kt
│   ├── model
│   │   ├── CategoryEntity.kt
│   │   └── TaskEntity.kt
│   ├── service
│   │   ├── CategoryServiceImp.kt
│   │   ├── MainServiceImpl.kt
│   │   ├── SplashService.kt
│   │   └── TasksServiceImp.kt
│   └── util
│       ├── Constants.kt
│       └── safeCall.kt
├── design_system
│   ├── color
│   │   ├── darkThemeColor.kt
│   │   ├── lightThemeColor.kt
│   │   └── TudeeColors.kt
│   ├── component
│   │   ├── AlertBottomSheet.kt
│   │   ├── AppBar.kt
│   │   ├── button_type
│   │   │   ├── FabButton.kt
│   │   │   ├── NegativeButton.kt
│   │   │   ├── NegativeTextButton.kt
│   │   │   ├── PrimaryButton.kt
│   │   │   ├── SecondaryButton.kt
│   │   │   └── TextButton.kt
│   │   ├── CategoryBottomSheet.kt
│   │   ├── CategoryItem.kt
│   │   ├── DatePickerDialog.kt
│   │   ├── DayCard.kt
│   │   ├── DefaultTextField.kt
│   │   ├── HeaderContent.kt
│   │   ├── LabelIconBox.kt
│   │   ├── NavBar.kt
│   │   ├── NoTasksSection.kt
│   │   ├── ParagraphTextField.kt
│   │   ├── Priority.kt
│   │   ├── Slider.kt
│   │   ├── TabsBar.kt
│   │   ├── TaskCard.kt
│   │   ├── ThemeSwitch.kt
│   │   ├── TudeeSnackBar.kt
│   │   └── TudeeTopBar.kt
│   ├── resources
│   │   └── TudeeResources.kt
│   ├── text_style
│   │   ├── defaultTextStyle.kt
│   │   ├── Font.kt
│   │   └── TudeeTextStyle.kt
│   └── theme
│       ├── Theme.kt
│       └── TudeeTheme.kt
├── di
│   ├── appModule.kt
│   └── dataModule.kt
├── domain
│   ├── model
│   │   ├── Category.kt
│   │   └── task
│   │       ├── Task.kt
│   │       ├── TaskPriority.kt
│   │       └── TaskStatus.kt
│   ├── service
│   │   ├── CategoriesService.kt
│   │   ├── MainService.kt
│   │   ├── SplashService.kt
│   │   └── TasksService.kt
│   └── util
│       ├── DomainError.kt
│       └── Result.kt
├── MainActivity.kt
├── presentation
│   ├── categories
│   │   ├── CategoriesRoute.kt
│   │   ├── CategoriesScreenActions.kt
│   │   ├── CategoriesScreenEvents.kt
│   │   ├── CategoriesScreen.kt
│   │   ├── CategoriesScreenState.kt
│   │   └── CategoryViewModel.kt
│   ├── home
│   │   ├── composable
│   │   │   ├── CardOverView.kt
│   │   │   ├── NoTask.kt
│   │   │   ├── OverViewSection.kt
│   │   │   ├── SliderStatus.kt
│   │   │   ├── TaskSection.kt
│   │   │   ├── TitleOverView.kt
│   │   │   └── TopSlider.kt
│   │   ├── HomeActions.kt
│   │   ├── HomeEvent.kt
│   │   ├── HomeRoute.kt
│   │   ├── HomeScreen.kt
│   │   ├── HomeUiState.kt
│   │   └── HomeViewModel.kt
│   ├── navigation
│   │   ├── Screen.kt
│   │   └── TudeeNavGraph.kt
│   ├── shared
│   │   ├── MainViewModel.kt
│   │   ├── taskdetails
│   │   │   ├── TaskDetailsBottomSheet.kt
│   │   │   ├── TaskDetailsState.kt
│   │   │   └── TaskDetailsViewModel.kt
│   │   └── taskeditor
│   │       ├── TaskEditorActions.kt
│   │       ├── TaskEditorBottomSheetContent.kt
│   │       ├── TaskEditorBottomSheet.kt
│   │       ├── TaskEditorEvent.kt
│   │       ├── TaskEditorUiState.kt
│   │       └── TaskEditorViewModel.kt
│   ├── splash
│   │   ├── onboard
│   │   │   ├── OnboardingRoute.kt
│   │   │   └── OnboardingScreen.kt
│   │   ├── splashscreen
│   │   │   ├── SplashReoute.kt
│   │   │   └── SplashScreen.kt
│   │   └── viewmodel
│   │       └── SplashViewModel.kt
│   ├── tasks
│   │   ├── DatePicker.kt
│   │   ├── MonthHeader.kt
│   │   ├── SwipableTask.kt
│   │   ├── TaskDeleteButton.kt
│   │   ├── TasksRoute.kt
│   │   ├── TasksScreen.kt
│   │   └── viewmodel
│   │       ├── TasksScreenActions.kt
│   │       ├── TasksScreenState.kt
│   │       ├── TasksViewModel.kt
│   │       └── TaskUi.kt
│   ├── tasks_by_category
│   │   ├── TasksByCategoryEvents.kt
│   │   ├── TasksByCategoryRoute.kt
│   │   ├── TasksByCategoryScreenActions.kt
│   │   ├── TasksByCategoryScreen.kt
│   │   ├── TasksByCategoryScreenState.kt
│   │   └── TasksByCategoryViewModel.kt
│   ├── uimodel
│   │   └── TaskUi.kt
│   └── utils
│       ├── errorToMessage.kt
│       ├── EventListener.kt
│       ├── GetCurrentDate.kt
│       ├── getCurrentLocalDateTime.kt
│       ├── Mapper.kt
│       └── millisToLocalDateTime.kt
└── TudeeApp.kt

</pre>

