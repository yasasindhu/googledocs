		
<JobCard 
logo="https://images.pexels.com/photos/9130415/pexels-photo-9130415.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" 
roleName="designer" 
companyName="zemoso" 
location="hyderabad"/>
<h2/>
# Integrating code blocks
```javascript
const App = () => {
    // This is a comment!
    return 'I am returning a string';
}
```
You can use this guide to start using Skyflow’s APIs. If you’re setting up Skyflow for your team or business, check out our guide on [Role-Based Access Control](https://docs.skyflow.com/developer-portal/how-tos/how-to:-author-a-policy-and-control-access-to-your-vault/) which will help you add teammates to your account and manage their permissions. By the end of this guide, you will be able to:
* Create a vault that you can use to securely store and protect your sensitive data.
### **Integrating the DemoApp **
<Iframe url="https://tokenization-demo.skyflow.app/#/creditCard"
     width="1000px"
     height="1000px" />
* Create and authenticate a service account that you can use for secure API communication.
<Divider/>
### **Before you begin**
Log in to your Skyflow account. If you don't have one, click to [request one here](https://skyflow.com/contact_sales).
### **Create a vault**
<h1/>
*Vaults* are data storage units where you can store your application’s sensitive data. Skyflow vaults come with several privacy-preserving mechanisms out of the box, such as polymorphic encryption and de-identification, built to keep your data secure. Skyflow APIs enable you to interact securely with the data.
To create a vault, log into your Skyflow account and go to the Vault Templates tab in Skyflow Studio, as shown below:
![image alt text](https://lh6.googleusercontent.com/yogewOwQCVEZ0cizmLkmCI8P4NQcD6RX1MZ7tyCOvRKt1d4XvC3B7FqyIg6CE6mei-Qg9HGePREDnbRt2At_cJjJhBbLHrt6vbyuqEVEsAJjIVnD2zOn2n1VfyXqirDwDWkvBpOL=s0 "image alt text")
*Vault Templates* define the high-level schema of the vault, including the fields and their relations. For instance, the Customer Identity vault comes packaged with all the sensitive fields a business would typically want to collect about a customer (email, phone number, and so on). Skyflow has a few predefined templates to choose from based on popular use cases.
Select a template and click Create. If you have multiple workspaces, select a *Workspace* to create the vault in.
Upon creating the vault, you’ll be taken to the *Vault Browser*. The Vault Browser lets you manage the data in the vault. Note, your newly created vault will be empty to start.
![image alt text](https://lh6.googleusercontent.com/5JqANer5bFRdBJMqMx5aMBTFCuat-kSNRBw9xJ0J9qsA0y-eiNxjYwNMY-uvFe8zeXy9jYRmE5fIV8ZaUKHtzNSfMmpR9TglRZWkHFseYuw_JmpJh9hBQ7lqplENbW-XvtnMg1qr=s0 "image alt text")
### **Create a Service Account**
*Service Accounts* provide secure channels of communication between your application and your vaults. To create an API Service Account for your vault, follow the steps below:
##### **Prerequisites**
* You must be a Vault Owner on a vault to create a service account
* Install Python 3.5 or later.
* Install PyJWT, requests and cryptography libraries
##### **Step 1 : Create an API Service Account and assign a role to it.**
* Navigate to the settings tab and select a vault for which you would like to create a service account from the drop down list on the left.
* Select ‘Service Accounts’ under the IAM section, and then click on ‘New Service Account’
* Enter a name and description.
* Assign the service account a Vault Owner role from the drop down menu and click ‘Create.’ You can also assign any other role instead of the Vault Owner role in this step.
* Upon clicking Create, a *credentials.json* file will be downloaded to your local machine. Store this file securely as it contains a private key that will be used to sign your JWT bearer token.
Here is an example of the credentials.json file:
```json
{
"clientID": "y4b0fb0991b211eb9a5e9a757ffcc4b0",
"clientName": "Customer support agent web  app",
"tokenURI": "https://manage.skyflowapis.com/v1/auth/sa/oauth/token",
"keyID": "y4c9577c91b211eb9a5e9a757ffcc4b0",
"privateKey": "-----BEGIN PRIVATE KEY-----\nMIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQCihOlTU61VztBu\nDhQtEb.....oGBAMFEvPAM0arx3qn7C067\nMLVrW2H6PwGpiWNU86rHBMkuzriwzagtit130XN8KrHfYfSRUmOOw6h6T4aC85g0\nwC8SQXRntfoise0UWcSxfnyhfqlaUeN3BqhHl0zjRQjE8W9th9k16N0rTPBRmPGo\nrWELwcVHR6izoGgGBAdWAGVn\n-----END PRIVATE KEY-----\n"
* }
```
Note: The Workspace URL and the Vault ID mentioned in the service account page will be required as URL paths when integrating with vault APIs.
##### **Step 2 : Prepare your environment**
### **Integrating the  Video **
 <Iframe
            
url="http://www.youtube.com/embed/xDMP3i36naA"
          />
