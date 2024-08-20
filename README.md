# Travel Memory

`.env` file to work with the backend:

```
MONGO_URI='ENTER_YOUR_URL'
PORT=3000
```

Data format to be added: 

```json
{
    "tripName": "Incredible India",
    "startDateOfJourney": "19-03-2022",
    "endDateOfJourney": "27-03-2022",
    "nameOfHotels":"Hotel Namaste, Backpackers Club",
    "placesVisited":"Delhi, Kolkata, Chennai, Mumbai",
    "totalCost": 800000,
    "tripType": "leisure",
    "experience": "Lorem Ipsum, Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum, ",
    "image": "https://t3.ftcdn.net/jpg/03/04/85/26/360_F_304852693_nSOn9KvUgafgvZ6wM0CNaULYUa7xXBkA.jpg",
    "shortDescription":"India is a wonderful country with rich culture and good people.",
    "featured": true
}
```
 # steps to deploy the travel memoey application on the aws ec2 #

The TravelMemory application has been developed using the MERN stack. 

Objective:
- Set up the backend running on Node.js.
- Configure the front end designed with React.
- Ensure efficient communication between the front end and back end.
- Deploy the full application on an EC2 instance.
- Facilitate load balancing by creating multiple instances of the application.
- Connect a custom domain through Cloudflare.

Project Repository:
Access the complete codebase of the TravelMemory application from the provided GitHub link: https://github.com/UnpredictablePrashant/TravelMemory

 Tasks:
1. Backend Configuration:
- Clone the repository and navigate to the backend directory.

    
    



-The backend runs on port 3001. Set up a reverse proxy using nginx to ensure smooth deployment on EC2. 

 

- Update the .env file to incorporate database connection details and port information.

 
2. Frontend and Backend Connection:

- Navigate to the `urls.js` in the frontend directory.
    


- Update the file to ensure the front end communicates effectively with the backend.
 
   
3. Scaling the Application:
- Create multiple instances of both the frontend and backend servers.
 

- Add these instances to a load balancer to ensure efficient distribution of incoming traffic.


4. Domain Setup with Cloudflare:
- Connect your custom domain to the application using Cloudflare.
-http://rajetraveljourney.maaan.org.in/ -hit this to access the backend of the applicatio	
- Create a CNAME record pointing to the load balancer endpoint.
- Set up an A record with the IP address of the EC2 instance hosting the front end.


 

- Designed a deployment architecture diagram using [draw.io](https://www.draw.io/) to visualize the flow and connections.

 

