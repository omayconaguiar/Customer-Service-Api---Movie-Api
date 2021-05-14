# Login

> ## Success Case:

1. ✅ Receive a request **POST** in **/api/login**
1. ✅ Check required fields **email **and **password**
1. ✅ Validate field **email** is a valid email
1. ✅ Search for the user with the provided email and password
1. ✅ Generate an access token from the user ID
1. ✅ Update user data with the generated access token
1. ✅ Returns 200 with the access token

> ## Exception:
1. ✅ Returns 404 error if the API does not exist
1. ✅ Returns 400 error if **email** or **password** is not provided by the client
1. ✅ Returns error 400 if the field **email** is an invalid email
1. 401 Returns 401 error if it does not find a user with the data provided
1. ✅ Returns error 500 if an error occurs when trying to generate the access token
1. ✅ Returns error 500 if an error occurs when trying to update the user with the generated access token