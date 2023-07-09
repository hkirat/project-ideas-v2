
### Google docs clone
Google docs is an app that lets you create and store documents online. It also lets you collaborate with other people on the same document.

The basic function requirements
- Let the user sign up and login
- Let the user create a document
- User should be able to create a viewable and editable link to send to friends
- User should be able to see the changes made by other people in real time
- You should be able to handle clashes when 2 people edit the same document at the same time, and the document should be eventually consistent

### Backend Service 
- Simple backend that lets users sign up and sign in (users table)
- Lets users create a doc (docs table)
- Lets users create a viewable and editable link to send to friends (links table)
- A websocket layer that relays events for the same doc amongst users
- Implementing operational transforms to avoid clashes when 2 people edit the same document at the same time

### Frontend service
- A simple frontend in react similar to the google docs website. You can use any UI framework you want, but I would recommend using tailwindcss.
- Bonus points if you can use a rich text editor library like slatejs