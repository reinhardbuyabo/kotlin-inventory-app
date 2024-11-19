Inventory app
==================================

Solution code for Android Basics with Compose.

Introduction
------------

This app is an Inventory tracking app. Demos how to add, update, sell, and delete items from the local database.
This app demonstrated the use of Android Jetpack component [Room](https://developer.android.com/training/data-storage/room) database.
The app also leverages [ViewModel](https://developer.android.com/topic/libraries/architecture/viewmodel),
[Flow](https://developer.android.com/kotlin/flow),
and [Navigation](https://developer.android.com/topic/libraries/architecture/navigation/).

Pre-requisites
--------------

You need to know:
- How to create and use composables.
- How to navigate between composables, and pass data between them.
- How to use architecture components including ViewModel, Flow, StateFlow and StateUi.
- How to use coroutines for long-running tasks.
- SQLite database and the SQLite query language


Getting Started
---------------

1. Download and run the app.

# Room
- Components of Room:
1. Room Entities (tables)
2. DAOs (CRUD methods)
3. Database Class ()

## Creating an Item Entity
- An entity defines a table, a row is a instance of the entity class
- After having an entity, we can create DAOs to access the database.

## Creating the item DAO
- DAO is a pattern that you can use to separate the persistence layer from the rest of the application by providing an abstract interface.
- Conflict: For example, multiple places in the code tries to update the entity with different, conflicting, values such as the same primary key.
- There is no convenience annotation for the remaining functionality, so you have to use the @Query annotation and supply SQLite queries.
- With Flow as the return type, you receive notification whenever the data in the database changes.

## Creating a Database Instance 
- companion object, which allows access to the methods to create or get the database and uses the class name as the qualifier.
- Refer to docs

## Implementing The Repository
- ItemsRepository and Offline ItemsRepository.
- Implement AppContainer Class.
- Refer to docs.