<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project Setup</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1, h2, h3 {
            color: #333;
        }
        pre {
            background: #f4f4f4;
            padding: 10px;
            border-radius: 5px;
            overflow-x: auto;
        }
        code {
            background: #eaeaea;
            padding: 2px 4px;
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Project Setup</h1>

        <h2>Prerequisites</h2>
        <ul>
            <li>Node.js (v14 or higher)</li>
            <li>npm (v6 or higher)</li>
        </ul>

        <h2>Backend Setup</h2>
        <ol>
            <li>
                <p><strong>Navigate to the backend directory:</strong></p>
                <pre><code>cd backend</code></pre>
            </li>
            <li>
                <p><strong>Install dependencies:</strong></p>
                <pre><code>npm install</code></pre>
            </li>
            <li>
                <p><strong>Create a <code>.env</code> file in the <code>backend</code> directory and add the following environment variables:</strong></p>
                <pre><code>PORT=4000
MONGO_URI='your_mongo_uri'
JWT_SECRET='your_jwt_secret'
GOOGLE_EMAIL='your_google_email'
GOOGLE_PASSWORD='your_google_password'
EMAIL_FROM='your_email_from'</code></pre>
            </li>
            <li>
                <p><strong>Start the backend server:</strong></p>
                <pre><code>npm run dev</code></pre>
            </li>
        </ol>

        <h2>Frontend Setup</h2>
        <ol>
            <li>
                <p><strong>Navigate to the frontend directory:</strong></p>
                <pre><code>cd frontend</code></pre>
            </li>
            <li>
                <p><strong>Install dependencies:</strong></p>
                <pre><code>npm install</code></pre>
            </li>
            <li>
                <p><strong>Start the frontend development server:</strong></p>
                <pre><code>npm run dev</code></pre>
            </li>
        </ol>

        <h2>Proxy Configuration</h2>
        <p>The frontend is configured to proxy API requests to the backend server. This is set up in the <code>vite.config.js</code> file:</p>
        <pre><code>server: {
  proxy: {
    '/api': {
      target: 'https://cypher-fullstack-assingment.onrender.com',
      secure: false,
    },
  },
},</code></pre>

        <h2>Running the Application</h2>
        <ol>
            <li>
                <p><strong>Start the backend server:</strong></p>
                <pre><code>cd backend
npm run dev</code></pre>
            </li>
            <li>
                <p><strong>Start the frontend development server:</strong></p>
                <pre><code>cd frontend
npm run dev</code></pre>
            </li>
            <li>
                <p><strong>Open your browser and navigate to:</strong></p>
                <pre><code>http://localhost:3000</code></pre>
            </li>
        </ol>

        <h2>Build for Production</h2>
        <ol>
            <li>
                <p><strong>Build the frontend:</strong></p>
                <pre><code>cd frontend
npm run build</code></pre>
            </li>
            <li>
                <p><strong>Start the backend server:</strong></p>
                <pre><code>cd backend
npm start</code></pre>
            </li>
        </ol>

        <h2>Scripts</h2>
        <h3>Backend</h3>
        <ul>
            <li><code>npm run dev</code>: Starts the backend server with nodemon for development.</li>
            <li><code>npm start</code>: Starts the backend server.</li>
        </ul>
        <h3>Frontend</h3>
        <ul>
            <li><code>npm run dev</code>: Starts the frontend development server.</li>
            <li><code>npm run build</code>: Builds the frontend for production.</li>
        </ul>
    </div>
</body>
</html>
