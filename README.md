# Car Management Application

A web application built with Next.js that allows users to manage car records. Users can create, view, edit, and delete their cars with details like images, title, description, and tags. The app includes user authentication and search functionality for easy management of records.

## Features
- **User Authentication**: Sign-up and log-in functionality for users to securely manage their cars.
- **Car CRUD Operations**: Create, view, update, and delete car records.
- **Image Upload**: Support for up to 10 images per car.
- **Tagging & Descriptions**: Add descriptive information and tags (car type, company, dealer) for each car.
- **Search**: Search across a user's car collection based on title, description, and tags.
- **API Documentation**: Access comprehensive API documentation at `/api/docs`.

## Tech Stack
- **Frontend/Backend**: [Next.js](https://nextjs.org/) (React-based framework).
- **Database**: PostgreSQL,
- **Authentication**: Next-Auth.
- **Cloud Deployment**: Deployed on Vercel

## Screenshots
![Login Page](path/to/login-page-screenshot.png)
![Product List Page](path/to/product-list-page-screenshot.png)
![Product Detail Page](path/to/product-detail-page-screenshot.png)

## Getting Started

### Prerequisites
- Node.js and npm installed.
- MongoDB/PostgreSQL (or your chosen database).
- Cloudinary/S3 bucket for image uploads (if required).

### Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/car-management-app.git
    cd car-management-app
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Set up environment variables**:
    Create a `.env.local` file in the root directory and add your environment variables:
    ```env
    DATABASE_URL=<your_database_url>
    JWT_SECRET=<your_jwt_secret>
    CLOUDINARY_URL=<your_cloudinary_url> # or another service for image storage
    ```

4. **Run the application**:
    ```bash
    npm run dev
    ```

5. **Access the application**:
    Open [http://localhost:3000](http://localhost:3000) in your browser.

### API Endpoints
| Method | Endpoint           | Description                 |
|--------|---------------------|-----------------------------|
| POST   | `/api/users`       | Create a new user           |
| POST   | `/api/auth/login`  | User login                  |
| POST   | `/api/cars`        | Add a new car               |
| GET    | `/api/cars`        | List all user's cars        |
| GET    | `/api/cars/:id`    | View a particular car       |
| PATCH  | `/api/cars/:id`    | Update a car's details      |
| DELETE | `/api/cars/:id`    | Delete a car                |

### API Documentation
Full API documentation available at `/api/docs` (Swagger or Postman).

## Deployment
This app is deployed on [Vercel/Heroku](https://your-app-url.com). Visit the live version here: [https://your-app-url.com](https://your-app-url.com).

## Folder Structure
