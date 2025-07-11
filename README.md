# SSEC Gate Attendance System

A web-based attendance management system for Sree Sakthi Engineering College, designed to track staff and student entry/exit records.

## Features

- Secure login system with multiple user roles (Admin, Management, Gate)
- Real-time attendance tracking
- Staff management
- Student attendance monitoring
- Department-wise statistics
- Automated data cleanup

## Tech Stack

- Frontend: HTML, CSS, JavaScript, Bootstrap 5
- Backend: Python Flask (Serverless Functions)
- Database: MongoDB Atlas
- Hosting: Netlify

## Deployment Instructions

1. **Prerequisites**
   - Netlify account
   - MongoDB Atlas account
   - Git installed on your machine

2. **Environment Variables**
   Set the following environment variables in Netlify:
   ```
   MONGODB_URI=your_mongodb_connection_string
   ```

3. **Deploy to Netlify**

   Option 1: Deploy via Netlify CLI
   ```bash
   # Install Netlify CLI
   npm install netlify-cli -g

   # Login to Netlify
   netlify login

   # Initialize and deploy
   netlify init
   netlify deploy --prod
   ```

   Option 2: Deploy via Netlify UI
   - Fork/Clone this repository to your GitHub account
   - Log in to Netlify
   - Click "New site from Git"
   - Choose your repository
   - Configure build settings:
     - Build command: `pip install -r requirements.txt && python app.py`
     - Publish directory: `static`
   - Click "Deploy site"

4. **Database Setup**
   - Create a MongoDB Atlas cluster
   - Set up network access and database user
   - Update the MongoDB connection string in environment variables

## Local Development

1. **Setup Virtual Environment**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Development Server**
   ```bash
   netlify dev
   ```

## Project Structure

```
├── netlify.toml          # Netlify configuration
├── requirements.txt      # Python dependencies
├── netlify/
│   └── functions/        # Serverless functions
│       └── api.py        # API endpoints
├── static/               # Static files
│   ├── index.html        # Main HTML file
│   ├── admin.html        # Admin dashboard
│   ├── styles.css        # CSS styles
│   ├── app.js            # Main JavaScript
│   └── admin.js          # Admin dashboard JavaScript
└── README.md            # Documentation
```

## Security

- Authentication using JWT tokens
- Environment variables for sensitive data
- CORS protection
- Input validation and sanitization
- Regular security updates

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.#   S S E C - g a t e - a t t e n d a n c e - b a c k e n d 
 
 #   S S E C - g a t e - a t t e n d a n c e 
 
 
