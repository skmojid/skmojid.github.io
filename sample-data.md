# Sample data for initial setup

# Add this data to your Firestore collections after setup

# Projects Collection
projects:
  - id: sample-project-1
    title: "E-Commerce Platform"
    description: "A full-featured e-commerce platform built with React and Node.js. Includes user authentication, payment processing, and admin dashboard."
    tech: ["React", "Node.js", "MongoDB", "Stripe"]
    image: "https://via.placeholder.com/400x300/4F46E5/FFFFFF?text=E-Commerce"
    github: "https://github.com/username/ecommerce-platform"
    live: "https://ecommerce-demo.com"
    createdAt: "2024-01-15T10:00:00Z"

  - id: sample-project-2
    title: "Task Management App"
    description: "A collaborative task management application with real-time updates, drag-and-drop functionality, and team collaboration features."
    tech: ["Vue.js", "Express", "PostgreSQL", "Socket.io"]
    image: "https://via.placeholder.com/400x300/10B981/FFFFFF?text=Task+Manager"
    github: "https://github.com/username/task-manager"
    live: "https://task-manager-demo.com"
    createdAt: "2024-01-10T15:30:00Z"

  - id: sample-project-3
    title: "Weather Dashboard"
    description: "A responsive weather dashboard that displays current weather conditions and forecasts for multiple cities with beautiful data visualizations."
    tech: ["JavaScript", "HTML5", "CSS3", "Weather API"]
    image: "https://via.placeholder.com/400x300/3B82F6/FFFFFF?text=Weather+App"
    github: "https://github.com/username/weather-dashboard"
    live: "https://weather-demo.com"
    createdAt: "2024-01-05T09:15:00Z"

# Admins Collection (create after setting up Authentication)
admins:
  - id: [USER_ID_FROM_FIREBASE_AUTH]
    email: "admin@example.com"
    role: "admin"