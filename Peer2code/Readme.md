# Peer Share
Peer Share is a code pair platform where users can share an interactive editor and write code together. It has language support for C++, Java and python. This application is based on the concept of operational transformation which forms the basis for a shared editor. Video calling is also provided within this application. It has some similar features as provided by [HackerRank's CodePair]

## How to Run Locally
1. react-app-rewired start
1.a npm i cors
1.b npm i express
### Frontend:
2. cd editor && npm start
### Backend:
3.cd editor-backend && npm run dev


## How real time editing works:
Real time editing is a two-way binding between server and client. This means there is a need of listener on both client side as well as server side. This might look very simple(Make a web socket listener and update the document). But, it is not the case. What happens when both the users edited the document at the same time? In that case, there is a possibility of storing ambiguous document. To solve this issue, we can use Operational Transformation.



## Video Calling:
This project doesn't use any external plugins for video calling. Instead, it uses APIs provided by WebRTC standard.
 - A STUN server is used to get public IP address
 - A TURN server is used to relay traffic if direct connection(peer to peer) fails. Currently, 
   free TURN server is used for demonstration. 

## Languages currently supported:
   - C++
   - Java
   - Python 2.x

## Completed Features:
   - **Real Time Editing:** Edit code in a real time monaco editor. Input and output are also real time.
   - **Run code:** Run code against a custom test case in currently supported languages.
   - **Private Channel:** Only the users who have access to the unique URL can edit in the editor.
   - **Video Calling:** Users can interact via video calling.
   - **Rich text presence:** Highlight the cursor position of other user.

## Features ToDo List 
   - **Support for more languages:** Code pair currently supports C++, Java and Python.
   - **Select questions from HackerRank and run all test cases:** Users can select questions from HackerRank and run all test cases against it (Maybe HackerRank provides an API for running all test cases).
   - **Proctoring control:** Detect when any user leaves the tab.
   ## Contributors:
   `Vivek Upadhyay`
   `Yash Bihari`