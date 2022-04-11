# The_MaRK3t

## A couple environment variables need to be set up in order to get the app up and running

## In the server folder:
- (MONGODB_URI), A Mongo DB URI, I will add you guys to the database project. Alternatively on our next call we can set this up. 
- (MONGODB_LOCAL), A local instance which makes testing easy. 
- Install the mongo db extension for VS Code if this is your IDE of choice. Alternatively there is something called Robo3t, these tools exist to help see what is being stored in the databse and how, (the schemwe design)
- (JWT_SECRET), make anything for now
- (AWS_ACCESS_ID), when you set up a IAM_User and create a group, you should be given an access Key ID, we can go through and set up if needed
-  (AWS_SECRET_KEY), this is also generated when you create a IAM user. 
- (AWS_REGION), set to 'us-east-1'
- (AWS_API_VERSION), set to '2010-12-01'
- Next you need to set up a stripe account, 
- (STRIPE_SECRET_KEY), this is generated when you set up your account. 
- (STRIPE_REDIRECT_URL), for now set as http://localhost:PORT/stripe/callback, whatever port you are running the client side on.
- Finaly for now (set your PORT number as an env variable)


## In the Client folder
- Create a .env.local file
- In there store, (NEXT_PUBLIC_API), this http://localhost:PORT/api, where port is the port that the server is running on
- (NEXT_PUBLIC_STRIPE_KEY), this is also from the stripe set up
- (NEXT_PUBLIC_TARGET_CHIAN_ID), this is for ganache used for web 3 testing


## Once you install all packages running npm i in both client and server, you must also run truffle init in the client side. This is for web3 integration and testing. 

## very early stages but already quite a few moving pieces. 
