# FiServ Pre-requisite and Setup Guide

## Pre-requisite Guide

You will need to install the followig tools to run the FiServ demo locally.

- [git](https://git-scm.com/downloads)
- [node](https://nodejs.org/en/download/)
- [VS code](https://code.visualstudio.com/)

## Step by Step Guide


1.  Copy this FiServ github repo link: https://github.com/mhsumbal-coveo/FiServ.git
2. Open VS code
3. Click on 'clone Git repository'
![image](https://user-images.githubusercontent.com/104369481/177623981-7d136a87-467a-476e-be97-da2dde5045d2.png)
4. Paste the link in the pop up window:
![image](https://user-images.githubusercontent.com/104369481/177624229-2cd8a486-7a66-4c54-9708-3529c90d0e29.png)
5. Save the cloned repository 
6. Open the cloned respository from the pop up window.
![image](https://user-images.githubusercontent.com/104369481/177624606-47a288c9-b0c9-4bc4-a21f-a03845ae2852.png)
7. Open the Terminal tab > New Terminal
8. Run the command ```npm install``` in the terminal
9. Create a .env file in the root directory and add keys and values using the example.env file. For FiServ .env file, contact mhsumbal@coveo.com. For creating your own API Key, follow the [screenshots](https://github.com/mhsumbal-coveo/Headless-Training/blob/main/API-Key_Screenshots.md).
10. Wait for all the packages to install and then run the command ```npm start``` in the terminal
11. The browser will open up automatically and FiServ will run locally on localhost:3000.

## Video Guide
https://user-images.githubusercontent.com/104369481/177627393-f56cb0e2-d954-477f-b532-1faed83d4964.mp4

## Hosting

Follow the guide below to host it on Netlify

Add the [_redirects](https://github.com/mhsumbal-coveo/FiServ/blob/main/public/_redirects) in the public folder if you have an older version of FiServ. [Guide](https://ridbay.medium.com/react-routing-and-netlify-redirects-fd1f00eeee95)

- Install Netlify CLI using ```npm install netlify-cli -g``` (close the terminal after installation and open it again)
- Build the application ```npm run build```
- Deploy using ```netlify deploy --prod```. You will be asked to login for the first time and answer the questions as below.
  - Create & configure a new site
  - select team => ```<select the team it shows>```
  - site name => ```<name-of-your-poc>```
  - Publish directory => ```build```
  
 After hosting is complete, the website URL will show up in the terminal. 
 
 To re-deploy, follow the steps below.
- Build the application again ```npm run build```
- Deploy using ```netlify deploy --prod```
