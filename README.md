## Event sourcing with springboot

<!-- wp:paragraph -->
<p>In Event Sourcing you just capture user events and add them in database, you just keep adding new events for every user action and no record is updated or deleted in the database , just events are added. Along with the events you also add event data specific to the event. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>This way you maintain the history of user action. This is useful if your application has security requirements to audit all user actions. This is also useful in any application where you want the history of user actions (example github commits , analytics applications etc) and to know the current state of an entity , you just rerun the events through your code and get that.</p>
<!-- /wp:paragraph -->

- Create Stock entity
- Create EventSore
- Create EventService
- Create EventRepository
- Create Event interface and it's implementation i.e StockAddedEvent and StockRemovedEvent.


## Requirements
- JDK 1.8 or more download
- Maven 3.6.1 
- Greenwich.SR2

## How to run the starter project?
- To run the service: Start the Main applications.

- Adding some items to stock

![Screenshot from 2022-09-13 13-09-11](https://user-images.githubusercontent.com/85616604/189884983-ef749124-8e59-4c0d-9d98-5dc738fd7cbb.png)
![Screenshot from 2022-09-13 13-09-36](https://user-images.githubusercontent.com/85616604/189884992-6fab5fff-de91-4985-b81f-22c7ef029f70.png)
![Screenshot from 2022-09-13 13-10-22](https://user-images.githubusercontent.com/85616604/189884996-a4241117-50c9-463b-80d0-09cd4b3a2a47.png)

- You can check database records

![Screenshot from 2022-09-13 13-21-50](https://user-images.githubusercontent.com/85616604/189884945-17f46ac4-274e-4bfc-8f96-5c5d4b865654.png)

- You can get events on behalf of name parameter

![Screenshot from 2022-09-13 13-27-28](https://user-images.githubusercontent.com/85616604/189884904-6ccb90aa-00bc-484d-b77b-fa41a6dcc87d.png)

- You can find out the stock's state of any particular day

![Screenshot from 2022-09-13 13-47-32](https://user-images.githubusercontent.com/85616604/189884016-dc0e02dd-fca9-42af-84ec-4403a99e5008.png)

