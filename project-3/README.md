
### Google meet clone
Google meet is an app that lets you do video conferencing with other people. It also lets you share your screen with other people.

The basic function requirements
- Let the user sign up and login
- Let the user create a new meeting
- Other users should be able to join meeting by id
- Users should be able to share their screen
- Users should be able to mute/unmute themselves

### Backend Service
- Simple backend that lets users sign up and sign in (users table)
- Lets users create a new meeting (meetings table)
- A websocket layer that relays events from the users to each other, and the does the WebRTC handshake
- The same websocket layer can be used for chat as well

### Frontend service
- A simple frontend in react similar to the google meet website. You can use any UI framework you want, but I would recommend using tailwindcss.