# 🚀 fullStackProject

<p align="center">
  <img src="https://img.shields.io/github/license/H0NEYP0T-466/fullStackProject?style=for-the-badge&color=blue" alt="License">
  <img src="https://img.shields.io/github/stars/H0NEYP0T-466/fullStackProject?style=for-the-badge&color=yellow" alt="Stars">
  <img src="https://img.shields.io/github/forks/H0NEYP0T-466/fullStackProject?style=for-the-badge&color=orange" alt="Forks">
  <img src="https://img.shields.io/badge/Contributions-Welcome-brightgreen?style=for-the-badge" alt="Contributions Welcome">
  <img src="https://img.shields.io/github/issues/H0NEYP0T-466/fullStackProject?style=for-the-badge&color=red" alt="Issues">
</p>

A modern, full-stack web application built with the **MERN** (MongoDB, Express.js, React.js, Node.js) stack that enables users to submit enquiry forms and provides comprehensive data management capabilities. This project demonstrates professional-grade **CRUD** operations, state management with React hooks, RESTful API communication, and seamless MongoDB integration.

## 📋 Table of Contents

- [🚀 Installation](#-installation)
- [💻 Usage](#-usage)
- [✨ Features](#-features)
- [📁 Folder Structure](#-folder-structure)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🗺️ Roadmap](#️-roadmap)
- [🙏 Acknowledgements](#-acknowledgements)

## 🚀 Installation

### Prerequisites

Before running this project, ensure you have the following installed:
- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **MongoDB** (local installation or MongoDB Atlas)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/H0NEYP0T-466/fullStackProject.git
   cd fullStackProject
   ```

2. **Install frontend dependencies**
   ```bash
   npm install
   ```

3. **Install backend dependencies**
   ```bash
   cd src/Server
   npm install
   cd ../..
   ```

4. **Setup MongoDB**
   - Start your local MongoDB server, or
   - Use MongoDB Atlas and update connection string in `src/Server/index.js`

5. **Start the backend server**
   ```bash
   cd src/Server
   node index.js
   ```

6. **Start the frontend development server**
   ```bash
   # In a new terminal, from the project root
   npm run dev
   ```

7. **Access the application**
   - Frontend: `http://localhost:5173` (or the port shown in terminal)
   - Backend: `http://localhost:8000`

## 💻 Usage

### Basic Workflow

1. **Submit Enquiry**: Fill out the enquiry form with your name, email, phone number, and message
2. **View Enquiries**: All submitted enquiries are displayed in real-time in the admin section
3. **Update Enquiries**: Click the update button to modify existing enquiry details
4. **Delete Enquiries**: Remove unwanted enquiries with the delete functionality

### API Endpoints

```bash
# Get all enquiries
GET http://localhost:8000/enquiries

# Create new enquiry
POST http://localhost:8000/insert

# Update enquiry
POST http://localhost:8000/update

# Delete enquiry
POST http://localhost:8000/delete
```

### Sample Data Format

```json
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "phoneNumber": "+1234567890",
  "message": "This is a sample enquiry message"
}
```

## ✨ Features

### 🎯 Core Functionality
- 📝 **User-Friendly Forms**: Intuitive enquiry submission with real-time validation
- 📊 **Admin Dashboard**: Comprehensive view of all submitted enquiries
- ✏️ **CRUD Operations**: Full Create, Read, Update, Delete functionality
- 🔗 **RESTful API**: Well-structured backend API with proper endpoints

### 🎨 User Experience
- 🎨 **Modern UI/UX**: Responsive design powered by TailwindCSS
- ⚡ **Real-time Updates**: Instant feedback and data synchronization
- 📱 **Mobile Responsive**: Optimized for all device sizes
- 🔔 **Interactive Alerts**: User-friendly notifications for all actions

### 🛠️ Technical Features
- 🏗️ **Component Architecture**: Modular React components for maintainability
- 🌐 **API Integration**: Seamless frontend-backend communication via Axios
- 🗄️ **Database Integration**: MongoDB with Mongoose ODM
- ⚡ **Fast Development**: Vite for lightning-fast build and development

## 📁 Folder Structure

```
fullStackProject/
│
├── 📄 README.md                    # Project documentation
├── 📄 package.json                 # Frontend dependencies & scripts
├── 📄 vite.config.js              # Vite configuration
├── 📄 eslint.config.js            # ESLint configuration
├── 📄 index.html                  # Main HTML template
│
├── 📁 src/                        # Source code directory
│   ├── 📄 App.jsx                 # Main React component
│   ├── 📄 App.css                 # App-specific styles
│   ├── 📄 main.jsx                # React entry point
│   ├── 📄 index.css               # Global styles (TailwindCSS)
│   │
│   ├── 📁 components/             # Reusable React components
│   │   └── 📄 Form.jsx            # Enquiry form & admin interface
│   │
│   ├── 📁 assets/                 # Static assets
│   │   └── 📄 react.svg           # React logo
│   │
│   └── 📁 Server/                 # Backend application
│       ├── 📄 index.js            # Express server entry point
│       ├── 📄 package.json        # Backend dependencies
│       │
│       ├── 📁 controller/         # Business logic
│       │   └── 📁 web/
│       │       └── 📄 controller.js   # CRUD operations
│       │
│       ├── 📁 model/              # Database models
│       │   └── 📄 enquiryModel.js     # Mongoose schema
│       │
│       └── 📁 routes/             # API routes
│           └── 📁 web/
│               └── 📄 enquiryRoutes.js # Route definitions
│
├── 📁 public/                     # Public assets
│   └── 📄 vite.svg               # Vite logo
│
└── 📁 dist/                      # Build output (generated)
    ├── 📄 index.html
    └── 📁 assets/
```

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### 🌟 Ways to Contribute

- 🐛 **Bug Reports**: Found a bug? [Open an issue](https://github.com/H0NEYP0T-466/fullStackProject/issues)
- 💡 **Feature Requests**: Have an idea? [Suggest a feature](https://github.com/H0NEYP0T-466/fullStackProject/issues)
- 📝 **Documentation**: Improve docs, add examples, or fix typos
- 🔧 **Code Contributions**: Submit pull requests for bug fixes or new features

### 📋 Contribution Guidelines

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/your-feature-name`
3. **Commit your changes**: `git commit -m 'Add some feature'`
4. **Push to the branch**: `git push origin feature/your-feature-name`
5. **Open a Pull Request**

### 🔍 Development Guidelines

- Follow existing code style and conventions
- Add comments for complex logic
- Test your changes thoroughly
- Update documentation if needed
- Ensure all linting passes

## 📄 License

This project is licensed under the **MIT License** - see the details below:

```
MIT License

Copyright (c) 2025 H0NEYP0T-466

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 🗺️ Roadmap

### 🎯 Upcoming Features

- [ ] 🔐 **Authentication System**: User login/registration with JWT
- [ ] ✅ **Form Validation**: Enhanced client & server-side validation
- [ ] 🌐 **Deployment**: Auto-deploy to Vercel (frontend) and Railway (backend)
- [ ] 🎨 **UI Enhancements**: Loading spinners, skeletons, and animations
- [ ] 🔔 **Notifications**: Toast notifications for better UX
- [ ] 📧 **Email Integration**: Email notifications for new enquiries
- [ ] 📊 **Analytics Dashboard**: Enquiry statistics and insights
- [ ] 🌙 **Dark Mode**: Theme switching capability
- [ ] 🔍 **Search & Filter**: Advanced enquiry search functionality
- [ ] 📱 **PWA Support**: Progressive Web App capabilities

### 🔄 Current Version: v1.0.0

### 📈 Version History

- **v1.0.0** - Initial release with basic CRUD operations
- **v0.9.0** - Beta version with frontend-backend integration
- **v0.5.0** - Alpha version with basic form functionality

## 🙏 Acknowledgements

### 🛠️ Built With

- [**React**](https://reactjs.org/) - Frontend library for building user interfaces
- [**Express.js**](https://expressjs.com/) - Fast, unopinionated web framework for Node.js
- [**MongoDB**](https://www.mongodb.com/) - NoSQL database for modern applications
- [**Mongoose**](https://mongoosejs.com/) - Elegant MongoDB object modeling for Node.js
- [**TailwindCSS**](https://tailwindcss.com/) - Utility-first CSS framework
- [**Vite**](https://vitejs.dev/) - Next generation frontend tooling
- [**Axios**](https://axios-http.com/) - Promise-based HTTP client

### 🎨 Design Inspiration

- Modern web design principles
- Material Design guidelines
- Responsive design best practices

### 👥 Contributors

- **H0NEYP0T-466** - *Initial work and project maintainer*

### 📚 Resources

- [MERN Stack Documentation](https://www.mongodb.com/mern-stack)
- [React Documentation](https://reactjs.org/docs)
- [Express.js Guide](https://expressjs.com/en/guide/routing.html)
- [MongoDB Tutorial](https://docs.mongodb.com/manual/tutorial/)

---

<p align="center">
  <strong>⭐ If you find this project helpful, please consider giving it a star! ⭐</strong>
</p>

<p align="center">
  Made with ❤️ by <a href="https://github.com/H0NEYP0T-466">H0NEYP0T-466</a>
</p>
