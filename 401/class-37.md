# Read: Class 37

## Reflections

The reading assignment explores Amazon S3 and its integration with Amplify for Android.

## Readings

[Introduction to Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)

1. What is Amazon S3?

    S3 stands for Simple Storage Service. It's Amazon's scalable storage service in the cloud.

2. List at least 3 features that it offers to its users.

    1. High durability and availability.
    2. Security features to manage data access.
    3. Options for data transfer, storage management, and monitoring.

3. What is an object key?

    An object key is the unique identifier of an object in an S3 bucket.

[S3 with Amplify](https://docs.amplify.aws/lib/storage/getting-started/q/platform/android/)

1. Which dependencies are needed to install Amplify AWS S3 to your Android application?

    The dependencies are `Amplify Framework` and `AWS S3 Plugin`.

2. What is needed in order to upload data to your bucket?

    You need to have the file/data, the bucket's name, and a unique key for the object.

3. what method(s) initialize(s) the Amplify Auth and Storage categories?

    The method is `Amplify.addPlugin()` for each category, followed by `Amplify.configure()`.

## Things I want to know more about

1. Interested in understanding more about best practices for managing and organizing data in S3.
