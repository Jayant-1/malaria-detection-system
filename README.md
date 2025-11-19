# 🩺 Malaria Detection System - Web Frontend

A modern, professional HealthTech web application featuring AI-powered malaria detection for hospitals. Built with React, Vite, TailwindCSS, and Framer Motion.

## ✨ Features

### 🎨 Design & User Experience

- **Clean, Modern Interface** - Professional HealthTech design with smooth animations
- **Dark/Light Mode** - Seamless theme switching with localStorage persistence
- **Fully Responsive** - Optimized for desktop, tablet, and mobile devices
- **Glassmorphism UI** - Modern frosted glass effects and gradient accents
- **Smooth Animations** - Powered by Framer Motion for fluid interactions

### 🔐 Authentication System

- **Role-Based Access** - Support for Doctors, Patients, and Admins
- **Elegant Forms** - Form validation with visual feedback
- **Persistent Sessions** - localStorage-based authentication

### 🏥 Role-Specific Dashboards

#### Doctor Dashboard

- Patient management and statistics
- Weekly test activity charts
- Monthly trend analysis
- Recent test results table
- Today's appointment schedule

#### Patient Dashboard

- Personal test history timeline
- Recent test results with detailed notes
- Upcoming appointments calendar
- Quick action buttons
- Health tips and recommendations

#### Admin Dashboard

- User distribution analytics
- System activity monitoring (24h)
- Monthly test analytics
- Recent user management
- System alerts and notifications

### 🤖 AI Detection Page

- **Drag & Drop Upload** - Intuitive image upload interface
- **Real-time Progress** - Animated progress bar during analysis
- **AI Simulation** - Mock AI analysis with realistic processing steps
- **Professional Results** - Color-coded diagnosis cards with confidence scores
- **Detailed Reports** - Comprehensive analysis details and metrics

### 📊 Data Visualization

- Interactive charts using Recharts
- Line charts for trend analysis
- Bar charts for comparative data
- Pie charts for distribution
- Real-time data updates

## 🚀 Tech Stack

- **React 19.2.0** - Latest React with concurrent features
- **Vite 7.2.2** - Lightning-fast build tool
- **TailwindCSS 4.1.17** - Utility-first CSS framework
- **Framer Motion 12.23.24** - Production-ready animation library
- **React Router 7.9.6** - Client-side routing
- **Recharts 3.4.1** - Composable charting library
- **Lucide React 0.553.0** - Beautiful icon library

## 📁 Project Structure

```
malaria-detection-system-web/
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── Alert.jsx
│   │   ├── Badge.jsx
│   │   ├── Button.jsx
│   │   ├── Card.jsx
│   │   ├── FeatureCard.jsx
│   │   ├── Footer.jsx
│   │   ├── ImageUpload.jsx
│   │   ├── Input.jsx
│   │   ├── LoadingSpinner.jsx
│   │   ├── Modal.jsx
│   │   ├── Navbar.jsx
│   │   ├── ProgressBar.jsx
│   │   ├── ResultCard.jsx
│   │   ├── Sidebar.jsx
│   │   ├── StatCard.jsx
│   │   └── TestimonialCard.jsx
│   ├── contexts/            # React contexts
│   │   ├── AuthContext.jsx
│   │   └── ThemeContext.jsx
│   ├── pages/              # Page components
│   │   ├── AdminDashboard.jsx
│   │   ├── DetectionPage.jsx
│   │   ├── DoctorDashboard.jsx
│   │   ├── HomePage.jsx
│   │   ├── LoginPage.jsx
│   │   ├── NotFoundPage.jsx
│   │   ├── PatientDashboard.jsx
│   │   └── RegisterPage.jsx
│   ├── App.jsx             # Main app component
│   ├── main.jsx            # Entry point
│   └── index.css           # Global styles
├── public/                 # Static assets
├── index.html             # HTML template
├── package.json           # Dependencies
├── tailwind.config.js     # Tailwind configuration
├── vite.config.js         # Vite configuration
└── README.md              # Documentation
```

## 🎨 Design System

### Color Palette

- **Primary**: Blue spectrum (#1890ff) - Trust and professionalism
- **Secondary**: Teal spectrum (#13c2c2) - Healthcare and vitality
- **Success**: Green for positive results
- **Danger**: Red for alerts and positive malaria cases
- **Warning**: Yellow for pending states

### Typography

- **Body Font**: Inter - Modern, highly readable
- **Display Font**: Poppins - Bold, impactful headings

### UI Elements

- Glassmorphism panels with backdrop blur
- Gradient accents and text effects
- Rounded corners (0.5rem - 1rem)
- Subtle shadows and hover effects
- 300ms transition animations

## 🛠️ Installation

1. **Clone the repository**

```bash
git clone <repository-url>
cd malaria-detection-system-web
```

2. **Install dependencies**

```bash
npm install
```

3. **Start development server**

```bash
npm run dev
```

4. **Open in browser**
   Navigate to `http://localhost:5173`

## 📝 Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run lint         # Run ESLint
```

## 🎯 Usage Guide

### For Doctors

1. Register/Login with Doctor role
2. Access Doctor Dashboard
3. View patient statistics and charts
4. Upload blood samples for detection
5. Review test results and manage patients

### For Patients

1. Register/Login with Patient role
2. Access Patient Dashboard
3. View personal test history
4. Request new tests
5. Track appointments and results

### For Administrators

1. Login with Admin role
2. Access Admin Dashboard
3. Monitor system activity
4. Manage users and permissions
5. View analytics and reports

## 🔒 Security Features

- Client-side authentication with role-based access
- localStorage for session persistence
- HIPAA-compliant design patterns
- Secure form validation
- XSS protection through React

## 🎭 Mock Data

The application currently uses mock data for demonstration:

- Simulated AI analysis (3-4 seconds)
- Random positive/negative results (70/30 split)
- Mock charts and statistics
- Sample patient and test data

## 🚀 Future Enhancements

- [ ] Backend API integration
- [ ] Real AI model connection
- [ ] JWT authentication
- [ ] WebSocket for real-time updates
- [ ] PDF report generation
- [ ] Email notifications
- [ ] Advanced analytics
- [ ] Multi-language support
- [ ] PWA capabilities
- [ ] Enhanced accessibility (WCAG 2.1)

## 📱 Responsive Breakpoints

- **Mobile**: < 640px
- **Tablet**: 640px - 1024px
- **Desktop**: > 1024px

## 🎨 Customization

### Updating Colors

Edit `tailwind.config.js`:

```js
theme: {
  extend: {
    colors: {
      primary: { /* your colors */ },
      teal: { /* your colors */ }
    }
  }
}
```

### Changing Fonts

Update Google Fonts import in `src/index.css`

### Adding New Routes

1. Create page component in `src/pages/`
2. Add route in `src/App.jsx`
3. Update navigation in `Navbar.jsx`

## 🐛 Known Issues

- ESLint warnings for unused motion imports (cosmetic)
- Mock data only - backend integration pending

## 👥 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- Design inspiration from modern healthcare platforms
- Icons by Lucide React
- Charts powered by Recharts
- Animations by Framer Motion

## 📞 Support

For questions or support, please contact:

- Email: contact@malariadetection.ai
- Website: Coming soon

---

**Built with ❤️ for Healthcare Innovation**

_Malaria Detection AI - Empowering Hospitals with Advanced Diagnostics_

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
