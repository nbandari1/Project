Homepage
>manage products
>PoS
>View past transactions
>Exit

>PoS
>Individual buttons for products
>Products will be displayed in a table when added
>When the payment button is pressed it will send it into a txt file with the date for past transactions
>It will then reduce the quantity of the products in the database by however much was taken away

>Manage products
>Allows user to add or take away products
>Allows them to add or reduce quantity

>View past transactions
>Displays a txt file of all the “receipts”


Functions

updateDatabaseQuantity

Called when the program initializes the payment
Parameters are productName quantity and a bool statement
Based on the bool statement, the function will change the product's quantity and add or take away. 
paymentAuth
When the button is pressed to authorize payment this function is called
The function will call updateDatabaseQuantity for each item in the receipt, and update the quantity.
The function will update a file called “records.txt” and add the information to it along with the date. (might be own function)
Clears the list and table of products

exportRecords
Takes in the list and price of the order
Adds it to records.txt file



Things that will be hard

Adding a button to for each product

Code that could help:
<div class="col-md-5"> <h2 style="font-size:25px;"> <?=$items['title'];?></h2> <img src="<?=$items['image'];?> "width='300' height='500'/> <p style="font-size:20px;" class = "lprice">GBP <?= $items['price'];?></p> <a class="btn btn-primary" href="add_to_cart.php?id=<?=$items['id'];?>">Add to Cart</a> </div>


