
# NVD CVE Information Management System

## Overview
The NVD CVE Information Management System is a web-based solution designed to efficiently consume, cleanse, manage, and visualize Common Vulnerabilities and Exposures (CVE) data from the National Vulnerability Database (NVD). This system helps organizations track and analyze software vulnerabilities by providing capabilities for data synchronization, retrieval, filtering, and visualization.

## Features
- **CVE Data Synchronization**: Automatically syncs CVE data from the NVD CVE API.
- **Search & Filter**: Allows users to search and filter CVE data based on various parameters like vulnerability type, severity, and affected software.
- **Data Visualization**: Provides an interactive user interface with visualizations to display the CVE data.
- **MongoDB Integration**: Stores CVE data in MongoDB for efficient querying and management.
- **Real-time Updates**: Ensures that the CVE database is up-to-date with the latest vulnerabilities and exposures.

## Technologies Used
- **Backend**: Flask (Python)
- **Frontend**: JavaScript (HTML, CSS, and Vanilla JavaScript)
- **Database**: MongoDB
- **API**: NVD CVE API (National Vulnerability Database)
- **Visualization**: Chart.js (for displaying vulnerability statistics)

## Installation

### Prerequisites
- Python 3.x
- Node.js (for managing JavaScript dependencies)
- MongoDB (local or cloud instance)

### Steps to Run the Project Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/nvd-cve-management.git
   ```

2. Navigate to the project directory:
   ```bash
   cd nvd-cve-management
   ```

3. Install backend dependencies:
   ```bash
   cd backend
   pip install -r requirements.txt
   ```

4. Configure MongoDB:
   - Ensure MongoDB is installed and running locally or use a cloud MongoDB service.
   - Update the `config.py` file with your MongoDB URI and API configurations.

5. Start the Flask backend:
   ```bash
   python app.py
   ```

6. Serve the frontend:
   - Navigate to the frontend directory:
     ```bash
     cd frontend
     ```
   - Open the `index.html` file in your browser or use a simple HTTP server:
     ```bash
     python -m http.server
     ```

7. Open the application in your browser at `http://localhost:8000` (if using `http.server`).

## Usage
- **Search CVE Data**: Use the search bar to query vulnerabilities by keyword or category.
- **Filter CVE Data**: Apply filters to view vulnerabilities by severity, affected software, or published date.
- **View Vulnerability Details**: Click on a CVE entry to see detailed information including description, risk, and links to more resources.

## Future Enhancements
- **Real-time Alerts**: Implement notifications or alerts for newly published CVEs.
- **Authentication**: Add user authentication for restricted access to certain features.
- **Data Export**: Enable export of CVE data to formats like CSV or Excel.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

