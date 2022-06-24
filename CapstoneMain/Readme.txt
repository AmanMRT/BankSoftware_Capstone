* REST End points

	HomePage
		http://localhost:8080/
		
	Account:
		http://localhost:8080/account/add													[Add New Account]
			Sample Input:
				{
					"accountType":"Savings",
					"accountbalance":500000.0
				}	
					
		http://localhost:8080/account/id													[Get Account Details by ID]
		http://localhost:8080/account/all													[Get All Accounts]
		http://localhost:8080/account/update/id												[Update Account Details]
		http://localhost:8080/account/delete/id												[Delete Account by Id]
		http://localhost:8080/account/transfer/fromAccount/toAccount/amount					[Transfer Fund from one account to another]
		
	Customer:
		http://localhost:8080/customer/add													[Add New Customer]	
			Sample Input:
				{
					"firstName":"Demo",
					"lastName":"DEMO",
					"phone":1234567890,
					"email":"demo@demo.com"
				}			
				
		http://localhost:8080/customer/id													[Get Customer Details by ID]
		http://localhost:8080/customer/all													[Get All Customers]
		http://localhost:8080/customer/update/id											[Update Customer Details]
		http://localhost:8080/customer/delete/id											[Delete Customer by Id]
		http://localhost:8080/customers/id/accounts											[Create account for Existing Customer]
			Sample Input:
				{
					"accountType":"Current",
					"accountbalance":200000.0
				}	
		