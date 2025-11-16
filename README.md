**🛍️ Online Boutique – Observability, Load Testing & Dashboard Integration**

📌 Assignment Overview

This repository implements Google’s microservices-demo application deployed on Kubernetes, with:

✅ Simulated traffic generation using Locust
✅ Visualization of logs, metrics, and traces using SigNoz
✅ Screenshots of Locust, SigNoz dashboards, and the application running locally
✅ Deployed SigNoz instance URL included
🔄 (Optional Bonus – persistence layer: add order storage in a database)

This work corresponds to the assignment instructions below:

Implement Google’s microservices-demo using Kubernetes (any cloud or self-hosted).
Generate traffic and visualize logs/metrics using SigNoz.
Bonus: Add a persistence layer and save order data.

**🔗 SigNoz Dashboard (Deployed)**

👉 URL: <YOUR_DEPLOYED_SIGNOZ_URL_HERE>
(Credentials / access shared separately as required)

**📸 Screenshots**
**🖥️ Application Running on Localhost**

**Home Page	Checkout Page**

<img width="1913" height="968" alt="image" src="https://github.com/user-attachments/assets/7a857d83-1329-4133-b85e-2cee222ce6cd" />
<img width="1910" height="963" alt="image" src="https://github.com/user-attachments/assets/11e5bda2-2d54-4f52-9b63-ee45f4f56b2b" />
	
**📊 SigNoz Dashboards
Services Overview	Traces	Metrics**

<img width="1918" height="972" alt="image" src="https://github.com/user-attachments/assets/967343a4-3fdd-4d45-860b-b321e0df8525" />
<img width="1917" height="964" alt="image" src="https://github.com/user-attachments/assets/edce6105-282a-4dda-9d99-792758d76a60" />
<img width="1918" height="962" alt="image" src="https://github.com/user-attachments/assets/824d28bf-baa0-40e3-a290-6cc90b99993d" />
<img width="1913" height="965" alt="image" src="https://github.com/user-attachments/assets/9cf096cc-24c5-45d8-8d3c-001cdaf21887" />
	
**🚦 Locust Load Testing
Locust UI	Charts	Stats**

<img width="1918" height="974" alt="image" src="https://github.com/user-attachments/assets/9c110ed1-c0af-42ee-bd13-cc6b90b88dd8" />

Online Boutique consists of 11 microservices communicating via gRPC:

Service	Language	Description
frontend	Go	Web UI
cartservice	C#	Redis-backed cart store
productcatalogservice	Go	Product catalog
currencyservice	Node.js	FX service
paymentservice	Node.js	Payment mock
shippingservice	Go	Shipping estimator
emailservice	Python	Email mock
checkoutservice	Go	Order flow
recommendationservice	Python	Cross-sell recommender
adservice	Java	Ad generator
loadgenerator	Python/Locust	Traffic generator
