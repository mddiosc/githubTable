# GitHub Repository Search Table

A Vue.js application that provides an intuitive interface for searching and browsing GitHub repositories using the GitHub REST API. Users can search for repositories with customizable filters and view detailed information in an organized table format.

## 🚀 Features

- **Search Functionality**: Search GitHub repositories by keywords
- **Advanced Filtering**: Sort results by stars, forks, updated date, and relevance
- **Responsive Design**: Mobile-friendly interface built with Vuetify
- **Detailed Repository View**: Expandable rows showing repository owner information
- **Pagination**: Server-side pagination for efficient data loading
- **Real-time Loading States**: Visual feedback during API requests

## 🛠 Technology Stack

- **Frontend Framework**: Vue.js 2.6.11
- **State Management**: Vuex 3.4.0
- **UI Framework**: Vuetify 2.2.11
- **HTTP Client**: Axios 0.21.1
- **Build Tool**: Vue CLI 4.5.0
- **Testing**: Jest with Vue Test Utils
- **Code Quality**: ESLint + Prettier
- **Date Handling**: Moment.js 2.29.1

## 📁 Project Structure

```
src/
├── components/
│   ├── SearchTable.vue      # Main search interface
│   ├── tableDetails/
│   │   └── RepoOwner.vue    # Repository owner details
│   └── ui/
│       ├── Header.vue       # Application header
│       └── Footer.vue       # Application footer
├── store/
│   └── modules/
│       └── github/          # GitHub API state management
└── styles/                  # Global styles and variables
```

## 🏗 Architecture Overview

The application follows Vue.js best practices with a modular architecture:

- **Component-based UI**: Reusable Vue components with clear separation of concerns
- **Centralized State Management**: Vuex store handles API calls and application state
- **API Integration**: RESTful communication with GitHub API v3
- **Responsive Design**: Mobile-first approach using Vuetify's grid system

## 🚦 Getting Started

### Prerequisites
- Node.js (v12 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd github-table
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run serve
```

4. Open your browser and navigate to `http://localhost:8080`

## 📝 Available Scripts

```bash
# Development server
npm run serve

# Build for production
npm run build

# Run unit tests
npm run test:unit

# Lint and fix files
npm run lint
```

## 🧪 Testing

The project includes comprehensive unit tests using Jest and Vue Test Utils:

- **Component Testing**: Tests for Vue components functionality
- **Store Testing**: Vuex actions, mutations, and getters validation
- **API Mocking**: Simulated GitHub API responses for consistent testing

Run tests with:
```bash
npm run test:unit
```

## 📊 Key Components

### SearchTable.vue
The main component that handles:
- Search form with filters (sort, order)
- Data table with pagination
- Repository results display
- Expandable rows for detailed information

### GitHub Store Module
Manages the application state including:
- API calls to GitHub REST API
- Repository data storage
- Loading states
- Error handling

## 🌐 API Integration

The application integrates with the GitHub REST API v3:
- **Endpoint**: `https://api.github.com/search/repositories`
- **Features**: Repository search with sorting and pagination
- **Rate Limiting**: Follows GitHub API rate limits
- **No Authentication**: Uses public API endpoints

## 🎨 UI/UX Features

- **Material Design**: Implemented using Vuetify components
- **Responsive Layout**: Optimized for desktop, tablet, and mobile
- **Loading States**: Visual feedback for API requests
- **Data Visualization**: Clear presentation of repository information
- **Accessibility**: WCAG compliant interface

## 📄 License

This project is available for educational and demonstration purposes.

---

Built with ❤️ using Vue.js and Vuetify
