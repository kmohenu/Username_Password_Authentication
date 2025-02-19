# Username_Password_Authentication
Basic Python Code for Username and Password Authentication
import getpass

user_name= "username"
passwd = "password"
# User requested to input Username and Password
#username = input("Please enter your username: \n ")
#password = getpass.getpass("Please enter your passwor>

# allows user to attempt login (Username and Password) Three (3) and locked out if unable to get correct username and password.
i=0
for  i in range(3):
        username = input("Please enter your username: \n")
        password = getpass.getpass("Please enter your password: \n")
        
        
        
        if username == user_name and password == passwd:
                print(f'Login successfull, Welcome: {user_name}')
        elif  i==2:
         
         print("You have had 3 Login tries, your account has been locked")

        else:
                print("login unsuccessful, incorrect username and password")
                print("Please try again")  
i=+1
