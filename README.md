# Chatroom_App is a web chat app. 
Users can go to the website at https://chat-application-274101.uk.r.appspot.com. 
Upon entering the correct username (admin) and password (camden) they are brought to a page where they can join a previously created room or create a new room. Upon joining a room the user is asked for their name, which is displayed for all other users to see when the user submits a comment. Other users are notified when someone joins or leaves a room they are in.

Technologies and languages used: Google Cloud App Engine, Javascript(ejs, express, npm, socket.io), HTML

Google Cloud App Engine - To deploy and host the chat app
Node.js - javascript runtime
ejs - embedded javascript html templates
express - web framework for server webpage communication
socket.io: enables communication between room participants


Security: There is only one username/ password hardcoded into the embedded java script. However, users can enter /room_list in the browser to get around requiring the credentials. This is a loophole I need to fix. I also meant to allow users to create usernames and passwords for authentication. The hashed passwords would be hashed and kept in  a mysql database. 

Design: Minimalist

Overview:
Website includes index.js(login page), room_list.js(list of available rooms to join or create new room), room.js(actual chat room), app.yaml(necessary for google cloud), package.json(includes dependencies), server.js(controls message passing), script.js(website logic)
