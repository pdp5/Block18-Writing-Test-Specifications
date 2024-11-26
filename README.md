# Block18-Writing-Test-Specifications

Block 18: WorkShop
Unit Tests:
1: A function called "multiplication" that returns the product of the two input numbers.
-Expect multiplication(2,3) to be a number
-Expect multiplication(2,3) to be equal to 6
-Expect multiplication("a",3) to be an error
-Expect multiplication(2) to be an error
-Expect multiplication(-2,3) to be equal to -6
-Expect multiplication(null,3) to be an error
-Expect multiplication(0,3) to be equal to 0
-Expect multiplication(infinity,3) to be an infinity
-Expect multiplication() to be an error
-Expect multiplication(2.5,3) to be equal to 7.5

2: A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays:
-Expect concatOdds([1,2],[-1,-3]) to be [-3,-1,1]
-Expect concatOdds([1,2,3],[-2,3]) to be [1,3]
-Expect concatOdds([24],[-2]) to be []
-Expect concatOdds([]) to be an error
-Expect concatOdds([],[]) to be []
-Expect concatodds("",[1,3]) to be an error
-Expect concatOdds([2.5],[1]) to be [1]
-Expect concatOdds(null , [5,6]) to be an error

Functional Tests:
1: A shopping cart checjout feature that allows a user to check out as a guest(without an account), or as a logged-in user. THey should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.
-When the cart is empty, there should be a message displaying "Your cart is empty"
-when the cart is empty there should be no preceed to checkout button
-When the cart is not empty it should disply the proceed to checkout button
-After clicking the proceed to checkout button, it should ask the user if the user wants to sign in or continue as guest
-If the user clicks on the continue as a guest button, it should display the fields to enter the user's information including shipping and payment details
-If the user clicks on sign in button, then it should display a login form, with a forget password, and create a new account button
-If the user enters invalied email/password it should display the error message
-If the user clicks on forget password button, it should ask the user to enter an email address that is being used to create an account
-After entring an email addresss, it should display an error message if the user doesn't have an account associated with that email
-If the user clicks on create a new account button, it should display the create account form
-If the user clicks on sign in button, and enter incorrect information then it should display an error message
-After successfully logging in, the shipping and payment details should be auto-filled in the form
-If the information is not saved then it should ask the user to enter shipping and payment details
-If the payment details is not valid then it should display an error message
-If the payment is successfull, the user should redirected to the confirmation page with order details
-The user should receive a confirmation email as well
