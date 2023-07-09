
### Google drive clone
Google drive is an app that lets you store files online. It also lets you share your files with other people.

The basic function requirements
- Let the user sign up and login
- Let the user upload a new file (upto 1GB)
- Create a link for the file that users can send to their friends
- Bonus points if you allow access control via emails
- You should use some sort of pre-signed URLs to avoid uploading first to your server and then to the object store

### Backend Service
- Simple backend that lets users sign up and sign in (users table)
- Lets users upload a file. You can use an existing object store like S3 to do the same. (files table)
- Lets users create a viewable and editable link to send to friends (links table)
- Bonus points if you allow access control via emails (access table)

### Frontend service
- A simple frontend in react similar to the google drive website. You can use any UI framework you want, but I would recommend using tailwindcss.