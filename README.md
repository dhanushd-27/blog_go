# Team Shiksha - Golang Proof of Work

#### Blog app backend using Golang

##### 🚀 Tech Stack

- **Language:** Go 1.24.2
- **Framework:** Gorilla Mux (HTTP Router)
- **Database:** PostgreSQL with GORM (ORM)
- **Authentication:** JWT (JSON Web Tokens)
- **Environment Variables:** godotenv
- **Password Hashing:** golang.org/x/crypto


##### Setup and Installation

1. Clone the repository
```bash
git clone https://github.com/dhanushd-27/blog_go.git
```

2. Install dependencies
```bash
go mod download
```

3. Set up environment variables
  - Note: JWT_SECRET field shoudn't be empty
```bash
cp .env.example .env
# Configure your environment variables
```

4. Run the application
```bash
go run main.go
```

##### Project Structure

- controllers/
  - Request handlers and Logic

- db/
  - Database connection logic

- helper/
  - Utility and helper functions i.e (Cors Handler, JWT Auth Handler, Api Server Handler)

- middleware/
  - Auth middleware

- models/
  - Contains user and blog model

- routes
  - User routes and Blog routes are present here

##### Data Models

- **User**
  - User model contains ID, username, email and password

- **Blog**
  - Blog model has Id, Title, Content and UserId for reference

#### Images of Testing the app using postman

##### User Signup
![User Signup](./assets/user-signup.png)

##### User Login
![User Login](./assets/user-login.png)

##### User Login Set Cookie

![User Login with cookie](./assets/user-login-cookie.png)

##### Creating a Blog
![Create Blog](./assets/blog-created.png)

##### Fetch all blogs
![Fetch All Blogs](./assets/fetch-all-blogs.png)

##### Fetch a blog with Id
![Fetch Blog by ID](./assets/fetch-blog-using-id.png)