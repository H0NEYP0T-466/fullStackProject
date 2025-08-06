# User Enquiry Form - MERN Stack Project

A full-stack web application built with the **MERN** (MongoDB, Express.js, React.js, Node.js) stack that allows users to submit enquiry forms and manage submitted data. This project demonstrates **CRUD** operations, state management with React hooks, RESTful API communication, and MongoDB integration.

## 🧠 Features

- 📝 Users can submit an enquiry form with name, email, phoneNumber, and message
- 📋 Admin view displays all submitted enquiries
- 🛠️ Update and delete operations for entries
- 🧾 Frontend and backend fully connected using Axios
- 🪄 Styled using TailwindCSS for a responsive and modern design
- 🔄 Real-time feedback with alerts on actions

## 📁 Project Structure

```
/fullStackProject
│
├── /backend
│   ├── index.js           # Main server entry point
│   ├── db.js             # MongoDB connection logic
│   └── model.js          # Mongoose schema/model for enquiries
│
├── /frontend
│   ├── /src
│   │   ├── App.jsx       # React root component
│   │   ├── Form.jsx      # Enquiry form + admin table
│   │   └── index.css     # Tailwind styles
│   └── tailwind.config.js # Tailwind config file
│
├── package.json (backend) # Backend dependencies
├── package.json (frontend) # Frontend dependencies
```

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/H0NEYP0T-466/fullStackProject.git
cd fullStackProject
```

### 2. Setup Backend

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory:

```
MONGO_URI=mongodb://localhost:27017/enquiries
PORT=5000
```

Start the backend server:

```bash
node index.js
```

### 3. Setup Frontend

```bash
cd ../frontend
npm install
```

Start the frontend:

```bash
npm run dev
```

> **Note:** Ensure both frontend and backend servers are running concurrently.

## 🔧 Tech Stack

- **Frontend:** React.js, Axios, TailwindCSS
- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Tools:** Vite, Concurrently, Nodemon

## 📦 Dependencies

### Backend

- express
- mongoose
- cors
- dotenv

### Frontend

- react
- axios
- tailwindcss
- vite

## 💡 Future Improvements

- Authentication system for admin
- Form validations (frontend & backend)
- Deploy to Vercel (frontend) and Render or Railway (backend)
- Add loading spinners and skeletons
- Toast notifications for actions

## 🙌 Contributing

Contributions are welcome! Please fork the repository, make changes, and open a pull request.

## 📄 License

This project is licensed under the **MIT License**.
