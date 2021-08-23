# S3
***Amazon Simple Storage Service (Amazon S3) is storage for the Internet. It is designed to make web-scale computing easier***

## Advantages of using Amazon S3

***Amazon S3 is intentionally built with a minimal feature set that focuses on simplicity and robustness. Following are some of the advantages of using Amazon S3:***

- ***Creating buckets – Create and name a bucket that stores data. Buckets are the fundamental containers in Amazon S3 for data storage.***

- ***Storing data – Store an infinite amount of data in a bucket. Upload as many objects as you like into an Amazon S3 bucket. Each object can contain up to 5 TB of data. Each object is stored and retrieved using a unique developer-assigned key.***

- ***Downloading data – Download your data or enable others to do so. Download your data anytime you like, or allow others to do the same.***

- ***Permissions – Grant or deny access to others who want to upload or download data into your Amazon S3 bucket. Grant upload and download permissions to three types of users. Authentication mechanisms can help keep data secure from unauthorized access.***

- ***Standard interfaces – Use standards-based REST and SOAP interfaces designed to work with any internet-development toolkit.*** 

## Operations

***Following are the most common operations that you'll run through the API.***<br>

***Common operations***

- ***Create a bucket – Create and name your own bucket in which to store your objects.***

- ***Write an object – Store data by creating or overwriting an object. When you write an object, you specify a unique key in the namespace of your bucket. This is also a good time to specify any access control you want on the object.***

- ***Read an object – Read data back. You can download the data via HTTP.***

- ***Delete an object – Delete some of your data.***

- ***List keys – List the keys contained in one of your buckets. You can filter the key list based on a prefix.***


## Notes

- ***The Amplify Storage category provides an interface for managing user content for your app in public, protected, or private storage buckets. The Storage category comes with default built-in support for Amazon Simple Storage Service (S3). The Amplify CLI helps you to create and configure the storage buckets for your app. The Amplify AWS S3 Storage plugin leverages Amazon S3.***

- ***To setup and configure your application with Amplify Storage and go through a simple upload file example***