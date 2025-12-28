# CipherSQLStudio
A browser-based SQL learning platform with real-time query execution and AI hints
CipherSQLStudio is a browser-based SQL learning platform where students can practice SQL queries against pre-configured assignments with real-time execution and AI-powered hints.


1.Features
 Assignment Listing Page with difficulty level

 SQL Editor for writing queries

 Real-time SQL query execution using PostgreSQL

 Query result display

 AI-powered hint system (gives guidance, not solutions)

 Mobile-first responsive UI


2.Tech Stack
Frontend

React.js

Vanilla CSS / SCSS (mobile-first)

Backend

Node.js

Express.js

Database

PostgreSQL (SQL execution sandbox)

MongoDB (assignment storage – extendable)

Other Tools

REST APIs

Environment Variables


3. System Architecture

Frontend (React)
⬇
Backend API (Express.js)
⬇
PostgreSQL (Query Execution)
⬇
LLM API (Hint Generation)



4. Data Flow

User selects an assignment

Assignment details are fetched from backend

User writes SQL query

Query is sent to backend API

Backend executes query on PostgreSQL

Results or errors are returned to frontend

User can request AI hints if needed


5. Installation & Setup
Backend Setup
cd backend
npm install
node index.js

Frontend Setup
cd frontend
npm install
npm start


6. Environment Variables
Backend .env
POSTGRES_URL=postgresql://user:password@localhost:5432/ciphersqlstudio

Frontend .env
REACT_APP_API_URL=http://localhost:5000
