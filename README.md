<img src='https://repository-images.githubusercontent.com/183605059/394a7680-6b39-11e9-837e-5a6ddb717b57' width='64'>


Pakistan Logistics Management Information System (LMIS) is an electronic logistics management system designed, developed and implemented indigenously to infuse efficency in Pakistan public health landscape.  The system is government owned and sustained system, providing updated and reliable supply chain data for vaccines, contraceptives and TB drugs for past more than 8 years. The application has evolved to capture real-time inventory data and product pipeline information to enable it to act as a critical supply management tool; whereby forecasting, quantification, pipeline monitoring and stock management functions are being performed by various government departments based on LMIS data. Over the years the system has started to move in to the centeral stage where multiple vertical stand alone information systems are being interfaced with it to draw consolidated information/analysis across the entire public health supply chain spectrum. 

LMIS was launched in July 2011 through USAID support. However, since then multiple donors e.g. WHO, UNICEF, GAVI, DFID and Gates Foundation have remained involved in LMIS scale-up, capacity building and data use; signifying its larger ownership not only in government but also among donors and UN agencies. 

The system is GS-1 compliant, supports threshold-based triggers/alerts as well as includes all needed supply chain features esp. pipeline and sufficiency of stocks in months of stocks, coverage, slice and dice reports and more. The system offers Zero vendor lock-in (LAMP Stack) with technical capacity available in the open market at a lower cost.  For generating user driven analytics (apart from built in reports) the system makes use of the pivot table and MS-BI 360 (Not included). This is the first step towards decoupling the modules so expect configuration glitches, however later plug and play VMs will follow. 

Support is always handy support@lmis.gov.pk 

This tool was created by the USAID-funded GHSC-PSM Program implemented by Chemonics International. See README below for more info.

# LMIS inventory management Systems (IMS)
LMIS inventory management Systems (IMS) web based providing real-time, perpetual inventory balances and open fulfillment status. The IMS has a capability to act as one system across various stores at different geographical levels has capability to manage the end-to-end inventory transactions across the supply chain. This allows the IMS user to see available balances and all issues/dispatches, including pending actions to be completed. Users are offered other functions, such as warehouse capacity management, views to incoming pipeline supplies and batch management functions. The dashboards provide ample information about Months of Supply, Storage vs Space Occupation Trends, Capacity Occupation of the warehouse, and issue/consumption information. Alerts provided to the IMS user include shipment alerts on incoming supplies, and product expiry alerts.
<img src='https://github.com/pakistanlmis/inventory-management/blob/master/public/images/im.png' width='300'>

# Configuration details
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
