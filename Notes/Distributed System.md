# 20-11-2025

# RPC (Remote Procedure Call)

#### RPC itself is a Conceptual most likely people known as API Request for now. Why its called Remote Procedure Call, In my opinion since it call other services remotely to do something in its local system that required to process several data,

### I think most people currently implement a concept that called Microservices. Because of the core function can call the required services. but when other services down as an example i have 2 services, An Auth Services and An Payment Services, if Auth Services down, i still can make a payment because my Payment Services running on different nodes

# Two General Problems

#### This case mostly occurs where a first condition requires 2nd condition to meet first, in this case as an example was when making a payment in real life when you using digital payment (such as QRIS, Debit or etc), where the Cashier will ask you to pay and then waiting the result of the return when the payment occurs, If it success then they give you the item, and if not they won't. 

#### I'm thinking when it comes to a programming, maybe the simple scenario was if you actually hit a services that requires other values to validate and process. Starting with you sending a request of payment to your services, but you won't instantly give the item to your client, instead you will wait the response of the services. From there, then they will do what it should do. 

#### However, what if the services down and you won't receive anything response? What i'm thinking is maybe revert or using Transaction and then rollback so you each actor doesn't minus anything at all. I Assume Two General Problems Requires Transaction for better result instead of relying the response only. 