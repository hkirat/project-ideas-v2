
### Streamyard clone

Streamyard is an app that lets you stream from your browser to apps like twitch and youtube.
The way it works is that it lets you add multiple video sources and then it streams the video to the streaming platform.
It also lets you add overlays and other effects to the video.
You can check out the website here - https://streamyard.com/
The website allows you to add more than 1 person to the stream, but for this project, we will only be adding 1 person to the stream (so you dont have to worry about browser to browser comm).

The basic function requirements
 - Let the user sign up and login
 - Let the user create a live stream
 - In the live stream page, the user can see themselves and a bunch of overlays. They can add and remove themselves from the canvas, and the same thing for the overlays
 - There should be a go live button that when the user clicks, the stream starts streaming whats on the canvas to youtube
 - This would require for you to write a service that takes video feed from the end user, merges it with the overlays on the canvas and then streams it to youtube

### Backend Service 1
 - Simple backend that lets users sign up and sign in (users table) 
 - Lets users create a live stream (live streams table)
 - Lets users add overlays/themselves to the live stream (overlays table)

### Backend service 2
This service takes the input stream and the current set of overlays and converts this to an RTMP stream that needs to be forwarded to youtube
Frameworks you can use to achieve this include ffmpeg or gstreamer.
Read about how you can convert websocket/WebRTC video streams to rtmp

### Frontend
A simple frontend in react similar to the streamyard website. You can use any UI framework you want, but I would recommend using tailwindcss.