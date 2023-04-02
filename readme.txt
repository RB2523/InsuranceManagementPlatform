
  
   
       Insurance management platform 
	      
		  In the System we have 3 enitites
		      Clients
			  Insurance Policies
			  Claims
			  
			     
		    -----------------
			   Structure :-
			 
			  Project is structure in packages
			   We have following packages in our projects
			   
			   com  
			   com.controller
			   com.entity
			   com.exception
			   com.repository
			   com.response
			   com.security
			   com.utility
			   
			
			----------------  
			  Features :-
			 
			   1) Fetch all clients
			   2) Fetch a specific client by ID
			   3) Create a new client
			   4) Update a client's information
			   5) Delete a client
			   
			   6) Fetch all insurance policies
			   7) Fetch a specific insurance policy by ID
			   8) Create a new insurance policy
			   9) Update an insurance policy
			   10) Delete an insurance policy
			   
			   11) Fetch all claims
			   12) Fetch a specific claim by ID
			   13) Create a new claim
			   14) Update a claim's information
			   15) Delete a claim
			  
			  ----------------  
			   
			    Client Validation 
				1) name , city , state , country  can have only lower and upper case letters
				2) contactNo , pincode	can have only numbers
				3) contactNo must have 10 digits
				4) mandatory fields:-  name , city , state , country ,contactNo , pincode
		 
		 
				InsurancePolicy Validation
				1) mandatory fields:-  policyNumber , policyType , policyCoverageAmount , policyPremium ,policyStartDate , policyEndDate
				2) policyCoverageAmount , policyPremium	can have only numbers
		  
				Claims Validation
				1) mandatory fields:-  claimNumber , claimDate , claimStatus 
				2) claimNumber can have only numbers
				3) claimStatus can have only lower and upper case alphabets
				
			 ----------------  
			  
			  Security 
			  
			  Basic authentication is implemented with 
			  userName = ram   
			  password = ram
				
			 ----------------  
			 
			 1) Follow Object oriented Approach
			 2) Proper exception handling is implemented 
			 3) Proper validation output will also send in JSON format
			 4) All response are send in JSON format
			 5) Primary Key for all table all records will be automatic generated and Primary Key will be a UUID string
			 
			 
			 ----------------  
			 How to run the application locally
			 1) Extract project
			 2) Open STS or any IDE capable or running spring boot project
			 3) File > Import
			 4) General > Existing project into Workspace
			 5) Browse the location where you have extracted the folder > select the folder > finish 
			  (Make sure you are connected to internet because it will download necessary dependency required to run project)
			 6) Install MYSQL in your system
			 7) In src/main/resource you get Application.properties file 
			 8) Chanage these 2 property in it according to your MYSQL username and password
			    spring.datasource.username
				spring.datasource.password 
			 9) Right click on  InsuranceManagementPlatform > Run as > Spring boot app
			 10) Open postman and can hit all the url in InsuranceManagementPlatform.postman_collection
			 
			 11) Just open postman and Export this file you get all 15 APIs
			 12) Remember to set basic authentication username and password mention above
			 
			 
				
			   
			
			   
			   
			   
			   