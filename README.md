# AI-Powered Process Monitor Dashboard

A modern, real-time system monitoring dashboard with AI-powered insights. Features dark mode support, live process monitoring, system metrics visualization, and intelligent analysis powered by Google's Gemini AI.

## 🚀 Features

### Real-time Monitoring
- Live process table with auto-refresh functionality
- Real-time system metrics graphs (CPU, Memory, Disk, Network)
- Process search and filtering capabilities
- Sortable columns for better data organization

### Process Management
- Process termination with confirmation dialog
- Priority adjustment (raise/lower)
- Process-specific analysis
- Export process list to CSV

### System Metrics
- CPU usage tracking
- Memory utilization
- Disk usage monitoring
- Network traffic analysis
- All metrics available in both light and dark modes

### AI-Powered Analysis
- Process behavior analysis using Gemini AI
- System health assessment
- Anomaly detection
- Performance optimization recommendations
- Resource usage patterns analysis

### User Interface
- Modern, responsive design
- Dark/Light mode toggle
- Real-time updates via WebSocket
- Interactive charts and graphs
- Intuitive process management controls

## 🛠️ Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- Google Cloud account with Gemini API access
- Modern web browser with JavaScript enabled

## 📦 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd process-monitor
```

2. Create and activate a virtual environment (recommended):
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/macOS
python3 -m venv venv
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up environment variables:
```bash
# Create .env file
touch .env  # or manually create it

# Add the following to .env:
GEMINI_API_KEY=your_api_key_here
FLASK_ENV=development
```

## 🚀 Running the Application

1. Start the development server:
```bash
python app.py
```

2. Access the dashboard:
```
http://localhost:5000
```

## 💡 Usage Guide

### Process Management
- **Search**: Use the search bar to filter processes by any field
- **Sort**: Click column headers to sort processes
- **Kill Process**: Select a process and click "Kill" (requires confirmation)
- **Priority**: Adjust process priority using "Raise Priority" or "Lower Priority"
- **Analysis**: Click "Analyze Process" for AI-powered insights

### System Monitoring
- **Metrics**: View real-time system metrics in the "System Metrics" tab
- **Refresh**: Click "Refresh" or wait for auto-refresh (2-second intervals)
- **Export**: Download process list as CSV using "Export CSV"
- **Theme**: Toggle between light and dark modes

### AI Analysis Features
- **Process Analysis**: Get detailed insights about specific processes
- **System Analysis**: Click "Analyze System" for overall health assessment
- **Recommendations**: Receive AI-powered optimization suggestions
- **Anomaly Detection**: Automatic identification of unusual behavior

## 🔒 Security Considerations

- Run with appropriate system privileges
- Store API keys securely in .env file
- Be cautious when terminating system processes
- Monitor API usage to stay within quotas
- Regular security audits recommended

## 🛠️ Technology Stack

### Backend
- Flask (Web Framework)
- psutil (System Monitoring)
- Flask-SocketIO (Real-time Updates)
- Google Generative AI (Gemini)
- Python-dotenv (Configuration)

### Frontend
- HTML5 & Tailwind CSS
- Chart.js (Visualizations)
- Socket.IO (Real-time Communication)
- Axios (HTTP Client)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Google Gemini AI for providing the AI capabilities
- Chart.js for the beautiful visualizations
- Tailwind CSS for the modern UI components
- The open-source community for various tools and libraries 