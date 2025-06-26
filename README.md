# Flutter technical test

This is a repository with a new flutter project, from the standard template.

## Required skills:

- **Basic english understanding** - This is because the apps we develop are targeted to the United States.
- **Good knowledge of object oriented programming** - Because we need a good code quality and maintainability.
- **Basic understanding of design patterns**
- **Good knowledge about basic software architectures**
- **A good understanding of the BLOC pattern** - using the `flutter_bloc` package
- **Good knowledge and understanding of firebase** (optional)
- **Experience with `go_router`**
- **Basic testing related knowledge** (optional) - Unit testing is enough, but integration tests are also good

## Required project
### Initial steps

Please add these items as issues to your repo and close them using commits or pull requests.

1. Fork this repository.
1. Set up app instrumentation with sentry or Firebase Crashlytics.
1. Set up the app with a `go_router` router.
1. Set up BLOC library.

### **Project requirements:**

The required app is the classic ToDo list.

Requirements are as follows:

- Feature requirements:
    - Tasks should be grouped.
    - Groups should be expandable in a main list view.
    - **Add Task** and **Add groups** should be separate screens
    - Task addition and group addition should refresh the group and task list.
    - Tasks without group should be listed next to task groups.
    - Tasks should have sub-tasks
    - Tasks and sub-tasks should be checkable
    - Tasks and sub-tasks should be editable.
    - User should be able to remove tasks and sub-tasks
    - User interface should be as clean as possible.
    - Ensure your project is usable by a screen reader user. (optional)
    - Add persistent storage (optional).
    - Add a settings page with access to an **About dialog** and a setting to switch between dark, light and system mode (optional).
- Code related requirements:
    - All screens of the application should be routable from the router.
    - Ensure you use a clean architecture or an hexagonal architecture. Either way, please use domain-driven-design when writing code.
    - Widgets shouldn't interact with service objects nor interfaces, they can only interact with BLOC objects.
    - BLOC objects shouldn't interact with any interface, just to domain-level services.
    - Domain-level objects shouldn't interact with concrete objects, they can only interact with interfaces when querying or saving data or doing any call to external API.