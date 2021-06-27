High Level System Design(HLD)
Requirement: Handle more customer
	Optimise processes and increase throughput using same resource
Name:	Pizza parlour

Pre:
	1 Chef
	
1. Preprocessing and Cron Job
	Preprocess material required during cooking, so cooking time can be reduced with same Chef
2. Keep backup and avoid single point of failure
	Employee backup chief incase main chief falls sick
3. Microservice
	Order pizza goes to Chef1 or Chef 3
	Order Garlic Bread goes to Chef 2
4. Distributed system, Partitioning
	Get more on pizza store, so incase it closes , power down
	Local location afenity
5. Load balancer, Routing
	Based on total time it will take customer to get the pizza
	queue time, time to make, time to deliver
6. Decoupling
	seprating manager for pizza and delivery
	decoupling the responsibility
7. Logging and Metrics
	Logg all operation, do reporting, metric and machine learning to enhance.
8. Extensible
	Dont need tro rewrite whole system if there is some change
		eg. Delivery guy does need to know if the deliverying Pizza today and tommorow Burger.

Low Level System Design(LLD)