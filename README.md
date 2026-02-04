# 💰 Money Manager Application

Welcome to the **Money Manager Application**! This is the frontend repository for a comprehensive full-stack project designed to help users take control of their finances with ease and precision.

Driven by a modern UI/UX, this application provides an interactive and seamless experience for managing income, expenses, and analyzing financial trends.

---

## 🚀 Key Features

This frontend application brings your financial data to life with the following features:

- **✨ Category Management**: Create, edit, and customize your own income and expense categories.
- **✨ Transaction Tracking**: Easily add, view, and delete income and expense transactions.
- **✨ Visual Analytics**: Interactive line charts that visualize data trends for the current month.
- **✨ Financial Overview**: Beautiful pie charts displaying a breakdown of total income, expenses, and current balance.
- **✨ Smart Filtering**: Quickly search and filter transactions using keywords to find exactly what you need.
- **✨ Recent Activity**: A dashboard view to see your latest transactions at a glance.
- **✨ Secure Authentication**: Built-in support for JWT power authentication flows (Login/Register UI).

---

## 📁 Tech Stack

This project is built using a modern, performant, and robust technology stack:

| Technology | Description |
| :--- | :--- |
| **React.js** | The core library for building the user interface. |
| **Vite** | Next Generation Frontend Tooling for fast builds and hot module replacement. |
| **Tailwind CSS** | A utility-first CSS framework for rapid and beautiful UI styling. |
| **Lucide React** | A collection of beautiful and consistent icons. |
| **React Hot Toast** | Polish interactions with smoking hot notifications. |
| **Recharts / React Charts** | Composable charting library for React components. |
| **Emoji Picker** | Fun and interactive emoji selection for categories. |

---

## 🛠️ Getting Started

Follow these instructions to get the project up and running on your local machine.

### Prerequisites

Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (Version 16 or higher recommended)
- [npm](https://www.npmjs.com/) (Node Package Manager)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/THATIPALLISAISHIVA/money-manager-client.git
   cd money-manager-client
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```
   > This will install all necessary packages listed in `package.json`.

3. **Configuration**
   Before running the application, you need to configure the backend connection and image upload settings in `src/util/apiEndpoints.js`.

   - **Backend URL**: Update the `BASE_URL` with your backend server URL.
   - **Cloudinary Setup**: Update the `CLOUDINARY_CLOUD_NAME` with your own Cloudinary Cloud Name for image uploads.

   Open `src/util/apiEndpoints.js`:
   ```javascript
   export const BASE_URL = "http://localhost:8080/api/v1.0"; // Set your backend URL
   const CLOUDINARY_CLOUD_NAME = "your-cloud-name"; // Set your Cloudinary name
   ```

### Running the Application

To start the development server:

```bash
npm run dev
```

The application will typically launch at `http://localhost:5173`. Open this URL in your browser to view the app.

### Building for Production

To create a production-ready build:

```bash
npm run build
```

---

## 📂 Project Structure

A quick look at the top-level files and directories you'll appreciate:

```
money-manager-client/
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable UI components
│   ├── pages/           # Page views (Dashboard, Login, etc.)
│   ├── services/        # API service calls
│   ├── context/         # React Context for global state
│   ├── assets/          # Images and styles
│   ├── App.jsx          # Main application component
│   └── main.jsx         # Entry point
├── index.html           # HTML template
├── package.json         # Dependencies and scripts
├── tailwind.config.js   # Tailwind CSS configuration
└── vite.config.js       # Vite configuration
```

---

