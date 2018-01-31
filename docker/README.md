# CI Project - Docker Part

## Process

I've just followed the next tuto : https://medium.com/@teeks99/continuous-integration-with-jenkins-and-gitlab-fa770c62e88a

Step 1 : Jenkins 
---------------------------

Add credentials on Jenkins credentials panel

    Kind        -> SSH Username with private key
    Private Key -> Your SSH id_rsa 


Step 2 : Gitlab
---------------------------

Create a token in "Access Token tab" in your Profile Settings

Copy your Personal Access Token 

Setp 3 : Jenkins
---------------------------

Add new credentials 

    Kind      -> Gitlab API Token
    API token -> Paste your Access Token

Then in Manage Jenkins/Configure System panel

Go to Gitlab section, set the Gitlab URL and the credentials

Now, in your project settings, fill the source code management section

And then fill the "Build Triggers" section

Step 4 : Gitlab
---------------------------

In your project settings, go to "Integration/Webhooks"

And now when you push whatever, a jenkins build will be starts
