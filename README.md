# Cost Manager RESTful Web Services

This project was developed as part of my Computer Science degree at HIT,  
in collaboration with [Dvir Uliel](https://github.com/DvirUliel).

It is a RESTful web service that manages cost tracking for users.  
The system provides APIs to add cost items, generate monthly reports, retrieve user details, and fetch information about the development team.

---

## Project Details
- **Database**: MongoDB (MongoDB Atlas)  
- **Framework**: Express.js, Mongoose  
- **Language**: JavaScript (Node.js)

---

## Features
- **Add Cost Items**: Add a new cost item to the database.  
- **Get Monthly Report**: Retrieve all cost items for a specific user in a given month and year.  
- **Get User Details**: Fetch the details of a specific user including their total costs.  
- **Get Developers Team**: Return a list of developers involved in the project.  

---

## Tools
- **Communication Tool**: Slack  
- **Issue Tracking**: Jira  

---

## Database Structure

**Users Collection**  
- `id`: Unique identifier  
- `first_name`: User's first name  
- `last_name`: User's last name  
- `birthday`: User's birthdate  
- `marital_status`: User's marital status  

**Costs Collection**  
- `description`: Description of the cost  
- `category`: Category of the cost (e.g., food, health, etc.)  
- `userid`: Reference to the user who incurred the cost  
- `sum`: Amount spent  
- `date`: Date when the cost was incurred  

---

## Endpoints

### `POST /api/add`
Adds a new cost item.  
**Request body**:
```json
{
  "description": "Description of the cost",
  "category": "Category",
  "userid": "User ID",
  "sum": 100
}

2. Deploy the server to a cloud platform like Heroku, AWS, or any other platform of your choice.

### License

This project is licensed under the MIT License.

