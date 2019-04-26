# inventory-management
/***************************** R E A D    M E ****************************/

For successfull running the module, kindly follow these steps:

1.Go to file : /includes/classes/Configuration.inc.php , and set your directory name in  : $system_main_path .

2. Restore this file on your mysql server : DB_RESTORE.sql

3.Go to file : /includes/classes/Configuration.inc.php , and set your DB credentials in following variables : 
				$db_host 		= '';
				$db_user 		= '';
				$db_password 	= '';
				$db_name 		= '';
				
				
4. Make sure your user is created .

5. For Creating New users , and warehouses, use the following credentials 
				User	= administrator
				Pass	= 123
				
6. Make sure , you create the warehouses first, Then you must assign those warehouses to the relevant users.
				
7. Now you are all set to log in.

/***************************** You Are Ready To Use ****************************/




A. If you wish to later integrate Email functionality, the configuration can be saved in : '/application/includes/classes/clsEmail.php'

B. If you wish to later integrate SMS functionality , configure it in the file: '/application/includes/classes/clsSMS.php'
