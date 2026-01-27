# Sample Data for SK MOJID Portfolio

Use this data to populate your portfolio after Firebase setup.

## Projects Collection

Add these sample projects to your Firestore `projects` collection:

```javascript
projects/
  project-id-1: {
    title: "E-Commerce Platform",
    description: "A full-featured e-commerce platform with user authentication, payment processing, product management, and admin dashboard. Built with modern web technologies and best practices.",
    tech: ["React", "Node.js", "MongoDB", "Stripe", "Tailwind CSS", "Firebase"],
    image: "https://via.placeholder.com/600x400/10b981/FFFFFF?text=E-Commerce+Platform",
    github: "https://github.com/skmojid/ecommerce-platform",
    live: "https://ecommerce.skmojid.com",
    createdAt: "2024-01-20T10:00:00Z"
  },
  
  project-id-2: {
    title: "Task Management System",
    description: "A collaborative task management application with real-time updates, drag-and-drop functionality, team collaboration features, and comprehensive project tracking dashboard.",
    tech: ["Vue.js", "Express.js", "PostgreSQL", "Socket.io", "Chart.js"],
    image: "https://via.placeholder.com/600x400/3b82f6/FFFFFF?text=Task+Management",
    github: "https://github.com/skmojid/task-manager",
    live: "https://tasks.skmojid.com",
    createdAt: "2024-01-15T14:30:00Z"
  },
  
  project-id-3: {
    title: "Weather Dashboard",
    description: "A responsive weather dashboard that displays current conditions, forecasts, and historical data for multiple cities with beautiful data visualizations and alerts.",
    tech: ["JavaScript", "HTML5", "CSS3", "Weather API", "Chart.js", "PWA"],
    image: "https://via.placeholder.com/600x400/8b5cf6/FFFFFF?text=Weather+Dashboard",
    github: "https://github.com/skmojid/weather-dashboard",
    live: "https://weather.skmojid.com",
    createdAt: "2024-01-10T09:15:00Z"
  },
  
  project-id-4: {
    title: "Social Media Analytics",
    description: "A comprehensive analytics platform for social media management with real-time data processing, sentiment analysis, and automated reporting features.",
    tech: ["React", "Python", "FastAPI", "Redis", "Docker", "PostgreSQL"],
    image: "https://via.placeholder.com/600x400/ef4444/FFFFFF?text=Social+Analytics",
    github: "https://github.com/skmojid/social-analytics",
    live: "https://analytics.skmojid.com",
    createdAt: "2024-01-05T16:45:00Z"
  }
```

## Admins Collection

After setting up Authentication, add your admin user:

```javascript
admins/
  [USER_ID_FROM_AUTH]: {
    email: "admin@skmojid.com",
    role: "admin",
    createdAt: "2024-01-01T00:00:00Z"
  }
```

## Contact Submissions

Example contact data (will be added automatically via the form):

```javascript
contacts/
  contact-id-1: {
    name: "John Doe",
    email: "john@example.com",
    subject: "Project Collaboration",
    message: "I'm interested in collaborating on a web development project. Let's discuss further.",
    createdAt: "2024-01-25T10:30:00Z"
  }
```

## Setup Instructions

### 1. Firebase Console Setup

1. **Authentication**
   - Go to Firebase Console → Authentication
   - Click "Add user"
   - Email: `admin@skmojid.com`
   - Password: `your-secure-password`
   - Copy the User ID from the user details

2. **Firestore Database**
   - Go to Firestore Database
   - Start collection: `admins`
   - Document ID: [paste User ID from step 1]
   - Fields:
     - email: `admin@skmojid.com` (string)
     - role: `admin` (string)

3. **Projects Collection**
   - Add each project from the sample data above
   - Use auto-generated Document IDs or create custom ones
   - Ensure all field types match the schema

### 2. Customization Tips

**Personal Information:**
```html
<!-- Update in index.html -->
<h1>Hi, I'm <span class="text-primary">YOUR NAME</span></h1>
<span>YOUR ROLE</span>

<!-- Update profile image -->
<img src="https://your-profile-image-url.jpg" alt="Your Name">
```

**Skills Section:**
```javascript
// Add your actual skills in assets/js/premium.js
const skillsData = {
    frontend: [
        { name: 'React', icon: 'fab fa-react', color: 'from-cyan-400 to-cyan-600' },
        { name: 'Vue.js', icon: 'fab fa-vuejs', color: 'from-green-500 to-green-600' },
        // Add your skills here
    ]
};
```

**Social Links:**
```html
<!-- Update in index.html and admin/index.html -->
<a href="https://github.com/YOUR_USERNAME" class="social-icon">
    <i class="fab fa-github"></i>
</a>
<a href="https://linkedin.com/in/YOUR_USERNAME" class="social-icon">
    <i class="fab fa-linkedin"></i>
</a>
```

### 3. Resume Setup

1. Upload your resume to a cloud storage service
2. Update the resume download link:
```html
<a href="https://your-resume-url.pdf" class="inline-flex items-center...">
    <i class="fas fa-download mr-2"></i>
    Download Resume
</a>
```

### 4. Contact Information

Update contact details in both portfolio and admin sections:
```html
<!-- In index.html contact section -->
<p class="text-neutral-600">contact@skmojid.com</p>
<p class="text-neutral-600">+91 YOUR_PHONE</p>
<p class="text-neutral-600">YOUR_CITY, India</p>
```

## 🚀 Next Steps

After setting up the sample data:

1. **Test Everything:**
   - Portfolio loading and navigation
   - Contact form submissions
   - Admin login functionality
   - CRUD operations for projects

2. **Personalize Content:**
   - Replace sample projects with your actual work
   - Update skills to match your expertise
   - Add your real contact information
   - Upload your profile photo and resume

3. **Deploy:**
   - Push to Netlify
   - Test live functionality
   - Set up custom domain (optional)

4. **Monitor:**
   - Check contact submissions regularly
   - Update portfolio with new projects
   - Monitor performance and user feedback

---

**Your premium portfolio is now ready to impress recruiters! 🎉**