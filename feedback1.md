# Avail Documentation Feedback 

## 1. Overview of Testing
- **Documentation Tested**: Avail `avail-js-sdk`
    Interacting on Avail
- **Purpose of Documentation**: To guide developers in setting up and using the `avail-js` library for working with the Avail blockchain.This Documentation helps developers to know how to interact with the network.
- **Testing Goal**: Verify the accuracy, clarity, and usability of the `avail-js` documentation by running through setup and sample usage.

## 2. Environment and Setup
- **Environment Used**:
  - OS Used:  Windows (using few devtools and docker)
  - Node.js version: 20.0
  - Additional tools: npm
- **Setup Instructions in Documentation**:
  - The documentation provided setup instructions for `avail-js-sdk` installation and initial configuration.

### Setup Experience
- **Observations and Issues Encountered**: Basically, The Prerequisite for `avail-js` were not clear enough and few things are missing. Like For Ex, you could provide an overiew of hosted endpoints more clearly.
-  I tried to work with hosted endpoints but was not getting appropriate response so ran a localnode
-  Running on Windows is preety tough when docker run doesn't work.
  
   ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av12.png)

-  it was giving manifest file error , so searched around docker registry to check avail image but i think avail image doesnt exists anymore on docker or couldn't find appropriate mapping.
  
   ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av11.png)
   
-  Another thing which i saw was generating an appId:-

   ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av13.png)

-  The Generator Web Application deployed on vercel is not working.its showing 404 Not Found, so either that deployment is revoked or something is missing.  
- **Resolved or Not**: I ran a local node by installing build tools and rust basically on windows, it took time but it worked at the end.for generating an appId I had to search for it and got end user guide,Understood about dataAvailability pallet,appKeys,nextAppId, so got to https://explorer.avail.so/#/extrinsics, https://explorer.avail.so/#/chainstate and resolved the issue . you could provide this url instead of that vercel url in interacting with avail-js blog.

  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av1.png)

  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av2.png)

  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av3.png)



## 3. Documentation Feedback
### Positive Aspects
- **Clarity**: Code-Examples and Expected Output Section were clear enough , when i was running few code examples it helped me to see expected output and current output. config.ts was also clear.
- **Avail - Js Connection and Transaction**- this main code spinnets helped me to explore github repository more clearly and looked for things bright enough.

  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av4.png)

  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av7.png)

### Areas for Improvement
- **Missing Steps or Details**:Docker Image is missing or its hidden dont know, AppID Generator Website on Vercel should be removed from blog's generating an appId blog section.
- **Ambiguous Language**: what is nom run transfer, i cannot say ambigious language but this few commands are incorrect this should be corrected.
  
  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/9cb1793b2cb1b88e42a74d05275bc598a7e7ef8b/Test_Images/av.png)

- **Suggestions for Improvements**: provide a docker image and also link to docker registry for troubleshooting purposes, and avail node setup was for ubuntu (linux) so we could focus on other os if not providing appropriate documentation for docker image.
  In future scope we can have avail.exe to run local node on windows.
  AppId should be explained more , and this websites should be depicted more enough 
  https://explorer.avail.so/#/extrinsics, https://explorer.avail.so/#/chainstate
  Like Avail-Js,can we provide documentation for avail-go,avail-deno setup. i got github - repo links for both. tried following that too , but that was not working so removed.
 
  ![](https://raw.githubusercontent.com/0xTaneja/AvailTestRepo/d58674974059b03c7ae1eeacb4a5846822b1ccff/Test_Images/av6.png)

  


