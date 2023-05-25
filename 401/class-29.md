# Read: Class 29

## Reflections

This reading assignment talks about Room, which is a library that provides an interface and abstraction layer to local SQLite database storage on a device for Android apps. Data persistence is obviously important for any application, so learning the options is relevant to growing our toolbox.

## Readings

[Overview: Saving data with Room](https://developer.android.com/training/data-storage/room)

[Defining entities in Room](https://developer.android.com/training/data-storage/room/defining-data)

[Related entities in Room](https://developer.android.com/training/data-storage/room/relationships)

[Accessing data with Room](https://developer.android.com/training/data-storage/room/accessing-data#java)

1. What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?

   Room is a persistence library that provides an abstraction layer over SQLite, a relational database engine. This is generally considered a good choice because SQLite is a lightweight, file-based database that is well-integrated into Android and provides full SQL capabilities. SQLite is great for mobile applications because it doesn't require a separate server process and allows for storing structured data locally on the device.

2. Do Rooms have any similarities to JPA?

    Yes, Room has some similarities to Java Persistence API (JPA), as both are abstraction layers over a relational database. They both provide ways to map Java objects to database tables (Object-Relational Mapping or ORM).

3. Describe a DAO in your own words

    A DAO, or Data Access Object, is an interface in Room that defines the methods for accessing the data in the database. In other words, it's a contract for how your application can interact with the database.

## Things I want to know more about

1. Is it generally the case that abstraction layers over databases are how almost all backend work is done? Or is the answer "it depends", as always?
