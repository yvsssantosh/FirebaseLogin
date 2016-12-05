# FirebaseLogin
This is a sample app made using Firebase which implements the login functionality

##Login Page
![](https://github.com/yvsssantosh/FirebaseLogin/blob/master/images/login_page.PNG)

##On clicking Sign-in with CORRECT credentials
![](https://github.com/yvsssantosh/FirebaseLogin/blob/master/images/login_with_correct_credentials.PNG)
	Here we are making a request to firebase engine and we are getting multiple responses from the same line.
	There seems to be no way to know programmatically, whether the user is actually logged in or not.
	Authentication state change occurs from **null** to **Logged in** and thus we are able to see the **logout** button

##On clicking Sign-in with INCORRECT credentials
![](https://github.com/yvsssantosh/FirebaseLogin/blob/master/images/login_with_incorrect_credentials.PNG)
	Here we are making a request to firebase engine but there incorrect user details i.e, **Login address** or **Password**.
	Authentication state change occurs from **null** to **Not logged in** and thus we are able to see the **logout** button.
	I think this must be refined in a better way to determine the exact login status.
	
##On clicking Sign-in with INCORRECT credentials and then with CORRECT credientials
![](https://github.com/yvsssantosh/FirebaseLogin/blob/master/images/login_with_incorrect_&_then_correct_credentials.PNG)
	Its natural that users might sometimes type their passwords incorrectly.So re-entering the password leads to this.
	Authentication state change occurs from **null** to **Not logged in** and thus we are able to see the **logout** button.
	But then we are unable to change its state even after entering the correct login details.
	
##On clicking Sign-in WITHOUT any credentials
![](https://github.com/yvsssantosh/FirebaseLogin/blob/master/images/login_with_no_credentials.PNG)
	True that there is nothing wrong with this but again there's change in Login state from **null** to **Not logged in** due to which we are able to see the logout button.
	
	

> **Note**: This is completely based on my observations and understanding on firebase which might not be true. People might have different answers to what I've posted here. So if I'm wrong....Please do correct me!
