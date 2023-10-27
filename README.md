# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
#### Step 1: 
Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

#### Step 2: 
Right-click on the project name and select New->RESTful Web Services from Patterns.

![2](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/cc8725f2-afe9-4a78-825e-36ee440d7f62)



#### Step 3: 
A new window will appear. Select “Simple Root Resource” and click Next.
 
![3](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/6b9e0dd7-2869-43ac-885a-a61515b84b77)



#### Step 4: 
In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![4](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/302e981a-3095-4330-a6ce-7b4052ce4f51)


#### Step 5: 
Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.

#### Step 6: 
Alter getHtml() method as shown below.

#### Step 7: 
Save your project, clean and build it. Deploy your project.
 
![7](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/046246cc-1882-4d48-949e-39d5d7f47ab9)

 

#### Step 8: 
To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).




### Client-Side:



#### Step 1: 
Create a new Java Web Project. Follow steps 1-5 as in section 1.1.

#### Step 2: 
Right-click on the project and select New->RESTful Java Client.

![c2](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/fdcb12ec-f208-4a97-8c73-19d10af3cc59)




#### Step 3: 
A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

#### Step 4: 
Carefully select your RESTful resource (web service) and click OK.
 
 ![c4](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/88fdda2e-1610-483a-81bf-ad3cdb749633)




#### Step 5: 
Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![c5](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/26bad541-a80b-48b5-ae9b-a07ce1f6ccf1)


#### Step 6: 
An editing tab will open. Alter getHtml() method with the following.
 
 ![c6](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/d1573e10-349d-42b7-81b7-e6af7c8130ac)




#### Step 7: 
Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![c7](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/9af372c9-6c04-45f9-8faf-1c76520eb83c)


#### Step 8: 
A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![c8](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/dd96bf70-8083-4b1d-9308-19f924e38e55)




#### Step 9: 
Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.


#### Step 10: 
A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![c9](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/3737c80e-59c7-4df7-a58e-c93637981c93)


#### Step 11: 
Save the project and build it.

#### Step 12: 
Run the JSP file and you should see the output in a new browser window.
 
 ![c12](https://github.com/Pandidharan/Ex-04_RESTful_Web_Services/assets/118343569/c27c6c9f-5415-4d43-a252-741eeb44704c)




### Client-Side Remote Invocation:



#### Step 1: 
Follow steps 1-5 as in Section 2.2

#### Step 2: 
In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";

#### Step 3: 
Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
