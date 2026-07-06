i did the attachment in brain station 23, from feb 20 to march 8. it lasted for around 2 weeks. i dont think i should mention the 2 week time span. what do you think?

as for the attachemt there were 7 of us. they made us submit full stack project proposal, and then they chose one. We then had 2 weeks to complete and deploy the project, and then showcase it.

- the project is a restaurant management software. restaurant owners can create one or more restaurants and manage their orders and inventory. Each restaurant gets their own url, upon visiting the site customers could get the menu and order online. this is the customer portal. 
- if orders are placed, waiters will be notified in the waiter porltal, waiter will then have to confirm the order by going to the table. we kept this manual step to protect from the misuse of the system, ie someone makes fake orders rtc.
- if orders are confirmed by waiter, chef will be notified by the chef portal, here chef will accept order, and update their state as cooking progresses. 
- waiter and chef portal uses websocket conn with backend to maintain realtime communication. multiple waiter, and chef, and waiter support is also implemented. as order status are updated, customer will also be notified by a socket connection. This conn is only created when a customer places order.
- finally, there is a management portal for restaurant owners, and managers. They could modify restaurant details, view food reviews, inventory. There were other management related features. 
- there was also an ai component. Here they are:
	- Recommendation: when a customer visits restaurant page he gets menu recommendation. If he's logged in then recommendations are tailored to them, otherwise they are based on previous sells. Owners can also promote orders, and these orders will have more weights when they are passed into the ai engine.
	- Review Analysis: food reviews are analyzed periodically to find out user complains about foods. food complains are aggregated and categorized into certain categories for easiler understanding of the management.
	- Sentiment Analysis: Get general user satisfaction level of a food item. This one focuses on finding out customer satisfaction while the previous one is specifically for finding out complains against foods.




- we were split into two teams, backend and frontend, and AI.  3 on frontend, 3 on backend, and 1 on ai.
- We analyzed the project then broke it into modules, such as auth, socket, payment, order management etc. We then assigned tasks to each member.
- I was the team lead of the backend and the architect of this project. I did the authentication, db schema design, project structure, websocket configuration, deployment, and some other modules. I also implemented the websocket connection in the fronend of customer, waiter and chef portal. 
- I basically managed the whole project, i helped all the other members. All the other members were less experienced in software dev than me. So i had to guide them all. During the last stretch, i had to fix a lot for frontend related issues, and worked on some fronend modules also.
- the ai team members developed the ai, and made a fastapi server to interect with the ai moduled. I integrated these modules into the backend. And then connected the ai module backend to the management.
- I also presented the project at the end.
- I dockerized the backend in the beginning. There were two reasons:
	- i tackled the deployment issue first, with the docker image i could then easily deploy the project
	- fronend team could work with the backend without any additional setup. They could just run the docker container, and use backend api. No additional config needed.


- We had daily scrum meeting everyday. We were working in a real corporate environment. We could ask mentors for any help. I learned a lot regarding architecture, deployment, project and people management.


So, as you can see I learned both technical and managarial stuff. But I have to say, i learned management more, and it was more fun this thime. Ususally Im a technical guy, but this time i had fun doing management, it's like i own the project, it's my responsibility to finish it. Even though i had to work on the fronend event though i was on that team, the fact that i finished it and presented is a win for me.

And, yeah, this was the industrial attachment experience for me.

