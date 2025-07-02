# TaskFlow Pro 🚀

A beautiful, feature-rich to-do list application built with React, TypeScript, and Tailwind CSS. Stay organized, meet deadlines, and achieve your goals with this modern productivity tool.

![TaskFlow Pro](https://images.pexels.com/photos/3184291/pexels-photo-3184291.jpeg?auto=compress&cs=tinysrgb&w=1200&h=400&fit=crop)

## ✨ Features

### 🎯 Core Functionality
- **Smart Task Management**: Add, edit, delete, and complete tasks with ease
- **Precise Scheduling**: Set both due dates and specific times for tasks
- **Priority System**: Organize tasks with Low, Medium, and High priority levels
- **Category Organization**: Group related tasks with custom categories
- **Automatic Status Detection**: Real-time overdue and due-today identification

### 🎨 Beautiful Design
- **Modern UI**: Clean, intuitive interface with smooth animations
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Color-Coded System**: Visual priority and status indicators
- **Gradient Backgrounds**: Eye-catching design that's easy on the eyes
- **Micro-interactions**: Hover effects and smooth transitions

### 📊 Analytics & Insights
- **Real-time Statistics**: Track total, pending, completed, and overdue tasks
- **Progress Visualization**: Beautiful progress bars and completion rates
- **Smart Filtering**: Filter by All, Pending, Today, Overdue, or Completed
- **Live Counters**: Dynamic task counts for each filter category

### 🔧 Advanced Features
- **Intelligent Sorting**: Automatic task prioritization by status, priority, and due date
- **Offline Support**: Works completely offline with localStorage persistence
- **Time-based Alerts**: Automatic overdue detection with visual warnings
- **Data Persistence**: Your tasks are automatically saved and restored

## 🚀 Live Demo

**[Try TaskFlow Pro Live](https://jazzy-pie-95e920.netlify.app)**

## 🛠️ Technology Stack

- **Frontend**: React 18 with TypeScript
- **Styling**: Tailwind CSS with custom animations
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Deployment**: Netlify
- **Storage**: Browser localStorage

## 📦 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd taskflow-pro
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

### Build for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## 🎮 How to Use

### Creating Tasks
1. Click "Add a new task..." to expand the creation form
2. Enter your task description
3. Set due date and time (optional)
4. Choose priority level (Low, Medium, High)
5. Add a category for organization (optional)
6. Click "Add Task" to save

### Managing Tasks
- **Complete**: Click the circle checkbox to mark as done
- **Edit**: Hover over a task and click the edit icon
- **Delete**: Hover over a task and click the trash icon
- **Filter**: Use the filter tabs to view specific task groups

### Understanding Visual Indicators
- 🔴 **Red Border**: Overdue tasks
- 🟠 **Orange Border**: Tasks due today
- 🟢 **Green Background**: Completed tasks
- **Priority Badges**: Color-coded priority levels
- **Category Tags**: Blue badges for task categories

## 📁 Project Structure

```
src/
├── components/           # React components
│   ├── AddTaskForm.tsx  # Task creation form
│   ├── EmptyState.tsx   # Empty state displays
│   ├── FilterTabs.tsx   # Filter navigation
│   ├── TaskItem.tsx     # Individual task component
│   └── TaskStats.tsx    # Statistics display
├── hooks/               # Custom React hooks
│   └── useTaskTimer.ts  # Timer for overdue detection
├── types/               # TypeScript type definitions
│   └── index.ts         # Task and filter types
├── utils/               # Utility functions
│   └── localStorage.ts  # Data persistence logic
├── App.tsx              # Main application component
├── main.tsx             # Application entry point
└── index.css            # Global styles
```

## 🎯 Key Components

### Task Interface
```typescript
interface Task {
  id: string;
  text: string;
  completed: boolean;
  createdAt: Date;
  completedAt?: Date;
  dueDate?: Date;
  priority: 'low' | 'medium' | 'high';
  category?: string;
}
```

### Filter Types
- `all`: Show all tasks
- `pending`: Show incomplete tasks
- `completed`: Show finished tasks
- `overdue`: Show past-due tasks
- `today`: Show tasks due today

## 🔄 Data Flow

1. **Task Creation**: Form data → Task object → State update → localStorage
2. **Task Updates**: User action → State modification → localStorage sync
3. **Status Detection**: Timer hook → Overdue check → Visual updates
4. **Filtering**: Filter selection → Task array filtering → UI update

## 🎨 Design Philosophy

TaskFlow Pro follows modern design principles:

- **Minimalism**: Clean interface without clutter
- **Hierarchy**: Clear visual organization of information
- **Feedback**: Immediate response to user actions
- **Accessibility**: Readable fonts and sufficient contrast
- **Responsiveness**: Seamless experience across devices

## 🚀 Performance Features

- **Optimized Rendering**: Efficient React component updates
- **Local Storage**: Fast data access without network calls
- **Lazy Loading**: Components load only when needed
- **Smooth Animations**: 60fps transitions and micro-interactions

## 🔧 Customization

### Adding New Priority Levels
1. Update the `Task` interface in `src/types/index.ts`
2. Modify priority handling in components
3. Add corresponding color schemes in Tailwind classes

### Custom Categories
Categories are user-defined and automatically saved. No code changes needed for new categories.

### Styling Modifications
All styles use Tailwind CSS classes. Modify the `tailwind.config.js` for theme customization.

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **React Team** for the amazing framework
- **Tailwind CSS** for the utility-first CSS framework
- **Lucide** for the beautiful icon set
- **Vite** for the lightning-fast build tool

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](../../issues) page
2. Create a new issue with detailed information
3. Include browser version and steps to reproduce

## 🎬 Video Guide

A comprehensive video tutorial is available showing all features and functionality. The video covers:

- Interface overview and navigation
- Creating and managing tasks
- Using filters and categories
- Understanding visual indicators
- Tips for maximum productivity

---

**Built with ❤️ using React, TypeScript, and Tailwind CSS**

*TaskFlow Pro - Stay organized, meet deadlines, achieve your goals* ✨