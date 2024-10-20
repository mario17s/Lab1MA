# Lab1MA

ZooApp - Zoo Animals Tracker

Short description:
The application manages a list of animals in a zoo.
The main page of the application will have the list of animals (only name + photo).
When an item is clicked, a new page will be displayed. This will contain all the details of the animal.
The application should allow adding a new animal, deleting an animal and updating the information of an animal.

Domain details:
The entity used in the application is Animal.
Each animal has a name, photo, age, description, caretaker name (employee of the zoo), date on which it has been brought to the zoo.
Name is a string, photo a .png file, age an integer, description a string, caretaker name a string and the brought date is a date in dd-mm-yyyy format.

CRUD:
create - on the main page, the app has a button "Add new animal". When it is clicked, the user is directed to a new page where he has to fill out a form with the details of an animal. Upon successful addition, the user
is redirected to the home page and an appropriate message is shown.
read - the main page only has the photo and name of each animal. User has to click on any item, and a new page is shown. The page contains all the details of an animal.
update - on the animal details page, the user can click the button "edit" and a new form is showed, already filled with animal's info. He can change some info and save the changes
delete - on the animal details page, the user can click the button "delete" and the animal will be removed. The user will be redirected to the main page.

Persistence details:
create, update, delete will be persisted on the server and the local db, as the app will be using them in order to show the user correct and consistent information

When device is offline:
for read it wouldn't be a problem, since the app will be saving the data in an array, and not querying the db all the time (in-memory storage).
regarding the other CRUD operations, they can be performed using the in-memory storage and then syncing with the backend when the device is online again.
The modified items will be flagged in order to know which one has to be updated in the db.

Design link: https://www.figma.com/board/FblQejG53eS1gQm04WDKj6/Lab1?node-id=0-1&node-type=canvas&t=XMZnsCBKE39LlzoH-0
