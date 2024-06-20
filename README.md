# UPES MART (Online E-Commerce Website)
This is an E-Commerce Website build for selling of any electronics products online.

I created this project for my college major to showcase my skills. I request that it not be used for sale.

Note:- This is a Sample Project for learning purpose, we have not much considered of web security.

### About

In this projects a user can visit the websites, registers and login to the website. They can check all the products available for shopping, filter and search item based on different categories, and then add to cart. They can add multiple item to the cart and also plus or minus the quantity in the cart. Once the cart is updated, the user can proceed to checkout and click the credit card payment details to proceed. Once the payment is success the orders will be placed and users will be able to see the orders details in the orders section along with the shipping status of the product.

The admin also plays an important role for this project as the admin is the one responsible for adding any product to the store, updating the items, removing the item from the store as well as managing the inventory. The admin can see all the product orders placed and also can mark them as shipped or delivered based on the conditions.

One of the best functionality that the projects include is mailing the customers, so once a user registers to the website, they will recieve a mail for the successful registration to the website, and along with that whenever a user orders any product or the product got shipped from the store, then the user will also receive the email for its confirmation.
Sometimes, if the user tried to add any item which is out of stock, them they will get an email one the item is available again the stock.

Note: The payment page is created only for demo purpose and its not fully integrated with any payment gateway. So for now any credit card details will be accepted and the demo orders will be placed.

## Highlights :--

### The users will get a mail to their registered mail Id during:-
- New User Registration
- Order Successfully Placed
- The Item was out of stock while exploring but now it got available in the store
- Successful shipment and delivery of the Item

### Technologies used:-
1. Front-End Development:
- HTML
- CSS
- Javascript
- BootStrap

2. Back-End Development:
- Java
- JDBC
- Servlet
- JSP

3. Database:
- MySql

### ================ Software And Tools Required ================
- : Java JDK
- : Eclipse java and developer EE (Enterprise Edition)
- : Apache Maven
- : Tomcat v8.0+
- : MySQL Server
- : MySQL Workbench

### ================= Dummy Database Initialization =================
STEP 1: Open MySQL Command Prompt or MySQL Workbench

STEP 2: Login to the administrator user of MySql:
	 ```mysql -u <username> -p``` (Enter Password if asked)

STEP 3: Copy paste and execute the MySQL Query from the following file:-
- Run the Sql Query From this file: [databases/mysql_query.sql](./databases/mysql_query.sql)

### ======GENERATING GMAIL APP PASSWORD [For Mailing Functionalities]========
Step 1: Create a gmail account or login to existing account in any browser

Step 2 : Go to [https://myaccount.google.com/security](https://myaccount.google.com/security) and check if 2 step verifications is enabled or not, enable it if not enabled

Step 3: Go to [https://myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords) and enter password if asked

Step 4: In Select an App Section: select Other (custom name) => enter "Ecommerce Store" => Generate

Step 5: After that it will generate 16 digits app password which you need to copy and save for future configurations.

Step 6: Done : Now continue to importing the project. [Don't share the above password generated to anyone]

### ========== Importing and Running The Project Through Eclipse  ==========

Step 1: Open Eclipse.

Step 2: Click On File > Import > Git > Projects From Git > Clone Uri > Paste The Repository Url Select master Branch > Next > Next > Finish.

Step 3: Go inside ```Java Resources > src > application.properties``` and update the values as below:
- a) Update value for db.username and db.password according to your installed mysql credentials.
- b) Update value for mailer.email and mailer.password, with the same email and app password that you generated earlier in above section [ NOTE:Actual gmail password will not work]

Step 4: Right Click on Project > Run as > Maven Build > In the goals field enter "clean install" > apply > run

Step 5: Right Click On Project > Build Path > Configure Build Path > Libraries > Remove and Update Any Libraries if Red Mark Exists > Finish.

Step 6: Right Click on Project > maven > update project > select force update > apply > close

Step 7: Tomcat Configurations:
- If Tomcat Server is not configured in Eclipse :
	-  Right Click On Project > Run As > Run On Server > Manually Define a new server > Select server type > select Tomcat v8.0+ > (Select Tomcat V8.0+ Installation Location If Asked) > Next > Add the current project > Finish.

- Else If Tomcat Server is already configured in Eclipse:
	- Right Click On Project > Run As > Run On Server > Select Tomcat Version > Next > Add the project > Finish.
		<p align='center'>or</p>
	- You can directly goto server tab, select the tomcat server and use the debug or run button to start the previously ran project

Step 8: Check Running The Site At  [http://localhost:8080/shopping-cart/](http://localhost:8080/shopping-cart/)

Step 9:  [To Change the Port, if getting error like 'port already in use'] Open The Server Tab > Double Click On Tomcat Server > Ports > Change The Port Number For Http/1.1 To 8083 > Close And Save. Now Start and you can access the project on [http://localhost:8083/shopping-cart/](http://localhost:8083/shopping-cart/)

Step 10: Default Username And Password For Admin Is "admin@gmail.com" And "admin"

Step 11: The default Username And Password For User Is "guest@gmail.com" And "guest"

## FAQ
**Question:1** Unable to Connect to Database?

**Answer:** Please check you have installed the mysql correctly and have updated the correct db details in application.properties file. Also you can try doing maven clean install and force update the project and restart.
<hr>

#### Some Screenshots for the project:
- Home Page
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/db8f8322-dfca-424f-a815-e493f6f37318)
- Login Page
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/dc9aefe2-ab29-4aea-8d96-626860a1ebf9)
- Register Page
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/2a56d6ac-37b2-46cd-93af-2b0616812b65)
- Category Wise Product Filter
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/d106527e-c289-4cd7-9bbd-2e99ae2ffcfa)
- Cart Items
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/d9202313-a8a9-4a03-9358-c6ac5731301d)
- Credit Card Payment
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/4f576a47-171c-4dff-b0b6-a1411007e8f2)
- Order Details & Status
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/08cc74b0-c3be-44b6-9354-45409fd7819b)
- User Profile
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/5bc17bdd-dac1-4610-8610-4b41eeea5a20)

- Admin Home
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/95cfc39c-2744-4cf7-9387-fe0a458a8b69)
- Stock Items
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/e6885401-c8d8-4305-80e1-c8fba4b77f7f)
- Shipped Items
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/b3dfb610-f18c-47dd-8027-4d5f7a51070e)
- Recent Orders yet to be shipped
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/561d3374-2bdc-4089-aea0-bffbe1756997)
- Add Product to the stock
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/ac8a8e2d-f768-4836-a7f3-f6c13791a68c)
- Remove Product from the stock
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/12267da3-c1d1-443c-a537-6cb5e24a75bf)
- Update the stock item
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/2d70c127-5a26-4497-a56e-bc695eee0f29)

- Sample Email for order placed
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/cec90b85-f365-4c08-9b0f-fac7a5af8717)

- Class Diagram
![image](https://github.com/akshayahuja15/EcommerceWebsite/assets/83705640/25ebcfc5-bdf0-46b7-86cb-d3495dafaea0)

#### "Suggestions and project improvement ideas are welcomed!"

<bold>Thanks a lot,</bold><br/>
                                                                                                        Project Leader<br/>
                                                                                                         <b>Akshay Ahuja</b>


#   E c o m m e r c e - j a v a - s e r v l e t - W e b s i t e  
 