# Vipps Developer Portal

These are the steps after you have received in the onboarding email from Vipps. You should have received proper credentials with username on email and password on the admin-phonenumber. Use those credentials to log into Vipps Developer Portal in either test or production.

# Step 1

We start with the typical Sign-in screen.

![Sign on screen](images/Vipps_sign_in.PNG?raw=true "Title")

You type in your username and password here. Please note that there's a difference in both production and test when it comes to Vipps Developer Portal:

## Test

* Vipps Developer Portal for **test**: https://apitest-portal.vipps.no/
* A username that looks like this: `username@testapivipps.no`
* A default password. For a password change please contact `integration@vipps.no`

## Production

* Vipps Developer Portal for **production**: https://api-portal.vipps.no/
* A username that looks like this: `username@apivipps.no`
* A default password. For a password change please contact `integration@vipps.no`

## Remember to log out of other Microsoft accounts

![Error Screen](images/Error-Screen.PNG?raw=true "Title")

If you see the error page similar to the one above:

1. Make sure that you are logged out of any Microsoft Office 365 accounts, or make sure you are in incognito mode or "private window" in your browser.
2. Make sure you are using the correct URL. Remember https://apitest-portal.vipps.no/ for test, and https://api-portal.vipps.no/ for production.

# Step 2

After an successful log-in you will see the account name up in the right corner of the screen ("TOM KVAM" in this example). In the left corner you have several tabs.
The **"MANAGE USERS"** tab allows you to add users.

![Add users](images/add_user_vipps_developer_portal.PNG?raw=true "Title")

# Step 3

The next tab **"PRODUCTS"** shows you the APIs you currently have. As you see from the picture below you can have several products and the possibility to test them out in Vipps Developer Portal.

![Products](images/products_vipps_dev.PNG?raw=true "Title")

Click on the **"TEST THE API(S)"** button:
![Test the Api(s)](images/Test_the_api.PNG?raw=true "Title")

Click on the "Try it"-button:
![Try it](images/Try_it_out.PNG?raw=true "Title")

Add the the proper keys to initiate your request (see the next step):
![Request Payment](images/Request_payment.PNG?raw=true "Title")

# Step 4

To get your API keys, open the **"APPLICATIONS"** tab and click on the unit with the number-identificator that fits your Salesunit. You will find both `client_id` and `client_secret`.

![keys Applications](images/keys_application.PNG?raw=true "Title")

Under the tab **"REGISTER APPLICATION"** it should say, marked in red:

'All existing products have been subscribed'

Under the profile tab (the account name at the top right, "TOM KVAM" in this example) you will find your two last keys.

![keys_profile](images/keys_profile.PNG?raw=true "Title")

You have the `Access Token` key on the top. You have to click "Show" on the right side to make the keys appear. And as marked, its the `Primary key` you are after. If the key for some reason does not work, then you can hit "Regenerate", right next to "Show".

The `Ocp-Apim-Subscription-Key` is right below the `Access Token` key. You have to click "Show" on the right side to make the keys appear. And as marked, its the `Primary key` you are after. If the key for some reason does not work, then you can hit "Regenerate", right next to "show".

The `MerchantSerialNumber` (MSN) is the number right next to the name of your Salesunit, `100848` in this example.

Now you should have `Client_id`, `Client_secret`, `Access_token`, `Ocp-Apim-Subscription-Key` and `SerialMerchantNumber`, and you can proceed with the payment flow.
