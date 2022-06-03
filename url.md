# Loan Management Service
### Get Loan details based on ID
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/loan-management/getLoanDetails/{loan-id}/{cust-id}
- Header: Authorization token
- Response: Loan details of customer
### Save RealEstate collaterals
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/loan-management/saveRealEstateCollaterals
- Header: Authorization token
- Request-Body : Collateral details as per schema
- Response: 201 created
### Save CashDeposit collaterals
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/loan-management/saveCashDepositCollaterals
- Header: Authorization token
- Request-Body : Collateral details as per schema
- Response: 201 created
### API Documentation
- Swagger UI documentation: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com:8080/loan/swagger-ui/index.html

# Collateral Management Service
### Get collateral based on customer id and loan id
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/collateral-management/getCollaterals/{loan-id}/{cust-id}
- Header: Authorization token
- Details of collateral associated with the loan
### Get collateral based on loan id
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/collateral-management/getCollaterals/{loan-id}
- Header: Authorization token
- Details of collateral associated with the loan
### API Documentation
- Swagger UI documentation: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com:8082/collateral/swagger-ui/index.html
# Risk Assessment Service
### Get collateral risk based on collateral id
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/risk-management/getCollateralRisk/{collateral-id}
- Header: Authorization token
- Response: Risk percentage of collateral
### API Documentation
- Swagger UI documentation: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com:8083/risk/swagger-ui/index.html

# Authorization Service
### Validate JWT token
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/auth-service/validate
- Header: Authorization Token
- Response: 200 or 403
### Login
- URL: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com/auth-service/login
- Request body: Username and password
- Response: JWT token
### API Documentation
- Swagger UI documentation: http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com:8081/auth/swagger-ui/index.html

# Eureka Dashboard
- http://pod1-lb-969ddc5f8d623b95.elb.us-west-2.amazonaws.com:8761
