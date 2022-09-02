# notification

---
#### Instructions
Your task is to simulate a notification system using OOP principals that you've learned. As this is only a simulation, we're using a csv file as a mock database (database folder) to store our newly created notifications. 

A notification record should have the following columns: 
1. UUID
   - You can use a UUID package for this
2. Notification Type
   - There are two different kinds of notifications 
     - Email
     - Push Notifications
3. Message
    - Content of the notification.
4. Receivers
    - Receivers refer to different user groups that will receive the notification
      - Users
      - Merchants
5. Published At
   - Date that the notification is to be published
   - Format should follow this `31/08/2022 9:16 PM`
6. Status
   - Status of the notification
   - Pending, Completed, Cancelled

#### Guidelines: 
1. You'll want to create different classes for Notification types. 
2. Install composer and make sure files / classes are autoloaded for the App folder. Make sure each class is namespaced. 
3. You can think of each column as a property within the notification class. 
4. In your index.php, create 5 push notifications, and 5 email notifications.
5. Use a service class (NotificationService) which takes in a notification object, and writes to the csv. 
6. You'll want to use a class which reads from the csv file and extracts the data out, store in memory, and display the notifications in a table. 
7. Status should be colored. Green for completed, Red for cancelled, and Gray for pending.
8. You can use Enums / look up tables for Receivers and Statuses.

#### Tips: 
1. Read up about how to create and write to a csv file. 
2. Read up / make use of Interfaces.

#### Extra mile:
1. Add a method / feature which differentiates between Email and Push Notifications. 