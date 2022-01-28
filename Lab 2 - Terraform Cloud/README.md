![image](https://user-images.githubusercontent.com/98493117/151415048-45bda2e2-74d8-41f7-8a37-5638f3164cd1.png)


# Author
Kevin Tuffner - River Point Technology


# Estimated Time to Complete Labs

30 - 45 Minutes


# Step # 1 - Setting up HashiCorp Terraform Cloud Account with your email address

We will sign up for a HashiCorp Terraform Cloud account using the following link:
http://app.terraform.io


![image](https://user-images.githubusercontent.com/98493117/151415346-b11dd452-e77b-438b-a214-45483cb9b61f.png)

*****************************************************************

# Step # 2 - Verify Terraform Cloud Account with your email address

Once we have signed up for the HashiCorp Terraform Cloud account, we will now need to verify our email address before we can utilize the platform

Lets log in with our newly created credentials when you registered for an account

![image](https://user-images.githubusercontent.com/98493117/151415571-3bdd5043-8f9c-4572-b4a9-c259b5464b99.png)

Please go ahead and confirm your email address. You will need to click confirm in an auto-generated email

![image](https://user-images.githubusercontent.com/98493117/151415695-e046ef52-6abf-4ec8-8f49-f03de57e259b.png)

*****************************************************************


# Step # 3 - Welcome to Terraform Cloud - Landing Page

Once we log in we should see this default landing page

** Update this picture ***

![image](https://user-images.githubusercontent.com/98493117/151415906-dbd2a101-50ec-44be-9148-64c0943379d7.png)

*****************************************************************


# Step # 4 - Log into Terraform Cloud via local laptop Terraform CLI

We need to setup our Terraform local CLI on our laptop with Terraform Cloud. Open up a terminal editor on your laptop and execute the "terraform login" command like the following screenshot. A new browser tab will open for you to create a Cloud API Token


<img width="685" alt="image" src="https://user-images.githubusercontent.com/98493117/151422121-32891f23-b58b-47e4-a65f-d7f3a52d7cf5.png">

*****************************************************************


# Step # 5 - Create Terraform Cloud API Token to be used with local Terraform CLI

<img width="487" alt="image" src="https://user-images.githubusercontent.com/98493117/151422462-e00e2f77-1949-4c49-9c9d-ddf2b3b2cbeb.png">

Enter a name for the Terraform Cloud API Token and then click create API Create Token. An API Token will then be created like the following screenshot.  Please copy this somewhere safe to be used in the next step with the local Terraform CLI

<img width="518" alt="image" src="https://user-images.githubusercontent.com/98493117/151422784-eb20c59d-1cc8-4ea6-be69-191b274e7a9c.png">

*****************************************************************


# Step # 6 - Enter Terraform Cloud API Token with local Terraform CLI

Lets go back to our terminal window and enter in our API Token that we just created and then click enter, and we will now be authenticated with Terraform Cloud using the API Token via our local Terraform CLI


<img width="623" alt="image" src="https://user-images.githubusercontent.com/98493117/151423113-e5edb94a-1925-4308-92f4-dd3a121cba25.png">


*****************************************************************


# Step # 7 - Create our first Terraform Cloud Organization Unit for the demo

Go back to our browser window for Terraform Cloud. Up in the top left corner, there will be a drop down menu next to the Terraform Logo where we can select create organization.  Click the create new organization and we will be now see the following screenshot down below


<img width="666" alt="image" src="https://user-images.githubusercontent.com/98493117/151423660-09602761-3795-4fb7-9c2e-6cd02eeb9c25.png">


Enter an "Organization Name" you want to use and then click Create Organization

We will now be re-directed to the workspaces web page and we should not see any workspaces created at this time

<img width="800" alt="image" src="https://user-images.githubusercontent.com/98493117/151424353-18f982f6-4497-4ee8-b9dd-0c9c74a2cc61.png">


*****************************************************************


# Step # 8 - Adding a VCS Provider in Terraform Cloud

Click on settings up on the top menu bar, and then on the left hand menu scroll down to Version Control, and then Providers. Click the Purple Control Button Called VCS Providers and we will then be presented with a new screen to choose our VCS Provider

<img width="713" alt="image" src="https://user-images.githubusercontent.com/98493117/151454423-4a86685b-f468-4179-9977-b8d825860608.png">


*****************************************************************

# Step # 9 - Choosing our VCS Provider to use in Terraform Cloud

We are going to use Github for this lab, so choose "Gitlab Custom"


<img width="656" alt="image" src="https://user-images.githubusercontent.com/98493117/151454581-77248cbe-6247-4d0c-94b4-fd80778140b7.png">



*****************************************************************

# Step # 10 - Setting up our VCS Provider in Terraform Cloud

We need to now click on the "register a new OAuth Application" under step # 1.  This link will then open a redirect to Github where we need to populate the details for Application Name + Homepage URL + Application Description + Authorization Callback URL. You can copy and paste these values from the Terraform Cloud window


<img width="688" alt="image" src="https://user-images.githubusercontent.com/98493117/151454788-945a8f8e-39eb-40e3-acc6-eaf711a05349.png">


*****************************************************************



# Step # 11 - Registering a new OAuth Application in Github for Terraform Cloud - Part # 1

Sample screenshot of the Github "Register a new OAuth Application" broswer tab

<img width="683" alt="image" src="https://user-images.githubusercontent.com/98493117/151454938-a1aadf60-db02-457f-95c3-df651b1498fb.png">


*****************************************************************


# Step # 12 - Registering a new OAuth Application in Github for Terraform Cloud - Part # 2

Filled in details from earlier steps

<img width="739" alt="image" src="https://user-images.githubusercontent.com/98493117/151455103-30b452b9-9d90-402f-bbf0-d8596e73538f.png">


*****************************************************************

# Step # 13 - Github OAuth Client ID and Secrets ID Details

We will need to copy the Client ID and also the Client Secret to our clipboard or IDE Editor to use in the next steps in Terraform Cloud


<img width="608" alt="image" src="https://user-images.githubusercontent.com/98493117/151456491-8c335b61-0b20-4b5b-b886-770f2a6ecbc6.png">


*****************************************************************


# Step # 14 - Populate Terraform Cloud VCS Provider Settings with Github Client ID and Secret ID Details

We will enter a name for this VCS Provider ( I used Github-Bridgecrew-Workshop)(we can name this anything) + We will enter the Github Client ID we copied earlier and also the Github Secret and then click "Connnect and Continue"


<img width="761" alt="image" src="https://user-images.githubusercontent.com/98493117/151456619-dc2dcc86-6977-4a09-8c46-a3bc91146850.png">


*****************************************************************


# Step # 15 - Authorize the Terraform Cloud VCS Provider and Github Application

A window will appear from Github asking for authorization. We will click the green button

<img width="655" alt="image" src="https://user-images.githubusercontent.com/98493117/151456747-aff8074a-4591-4b1c-8cf6-459406a554b2.png">



*****************************************************************


# Step # 16 - Additional Terraform Cloud VCS Provider Settings

We will skip this step since this is a workshop, but in a production setting you would setup a SSH Keypair to create an additional security barrier

<img width="641" alt="image" src="https://user-images.githubusercontent.com/98493117/151456901-83426ea2-6c62-4af6-8dfa-49496bbd784e.png">


*****************************************************************


# Step # 17 - Terraform Cloud VCS Provider Status

We should now see the status of our Terraform Cloud VCS Provider Configuration. Nothing to do here so we can move on to our next step

<img width="713" alt="image" src="https://user-images.githubusercontent.com/98493117/151457017-36235477-1d34-4df4-82d2-a07d78970724.png">


*****************************************************************

# Step # 18 - Getting started with Terraform Cloud Workspaces

Click on the workspaces link on the top navigation pane in Terraform Cloud.  Once this page loads then in the upper right hand corner there is a button for "new workspace" click on this.  You then will be directed to a new screen called " Create a new workspace" like the following screenshot down below.  In Terraform Cloud there are 3 workflow ways we interact with the Terraform Cloud Platform. 1) Version Contril Workflow (We are using this one today) + 2) CLI Driven Workflow + 3) API-Driven Workflow.  Click on the "Version Control Workflow"

<img width="834" alt="image" src="https://user-images.githubusercontent.com/98493117/151457220-bf6f06f7-2632-4f2e-9b14-0b82ddef57ac.png">


*****************************************************************



# Step # 6 - TBD TBD TBD

Select our workspace that will populate from our connected vcs provider

<img width="739" alt="image" src="https://user-images.githubusercontent.com/98493117/151475189-8db41c11-355a-4095-b99b-27073ac1dbe5.png">

*****************************************************************


# Step # 6 - TBD TBD TBD

<img width="698" alt="image" src="https://user-images.githubusercontent.com/98493117/151457627-f4067100-2a22-48f3-96d3-6dd10e6de34d.png">


*****************************************************************

# Step # 6 - TBD TBD TBD



