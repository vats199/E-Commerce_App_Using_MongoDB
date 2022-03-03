# E-Commerce_App_Using_MYSQL

SetUp instructions :- (First of all delete node_modules,package.json and package-lock.json files from this folder)

-> First of all install Node and npm on your system.
-> In terminal or cmd,create your own node_package using command 'npm init'. ('Visual Studio Code' Application is recommended to run your code)
-> After creating package you have to install some node libraries listed in packages.txt.
-> After installing the packages you have to add 1 command in your 'package.json' file :

                 add "start": "nodemon app.js" command in an object named "scripts" 

-> Create an account on MongoDB.
-> Then create an account on STRIPE and SENDGRID websites for adding a payment method and sending mails.                       
                        
-> After that you have to do some changes to the code in the given files :

            -> MongoDB_URL - app.js(16) (URL you can fetch from mongoDB website)

            -> SendGrid_API - controllers/auth.js(10) (API key you have to get from sendgrid account)

            -> Stripe - controller/shop.js(5) (Secret key you got from the stripe website)

                      - views/shop/checkout.js(26) (Publishable key you got from the stripe website)

            -> Encryption_Key - app.js (Any sentence you want as a key).....
