# API Testing Web App

A lightweight, browser-based API testing tool similar to Postman that allows you to test and manage HTTP/HTTPS requests. This tool runs entirely in the browser with no backend dependencies.

![API Testing Web App]
![image](https://github.com/user-attachments/assets/ae94031b-3421-4ad3-b84d-87df2eea35c9)


## Features

### 1. HTTP Request Support
- Supports all common HTTP methods:
  - GET
  - POST
  - PUT
  - PATCH
  - DELETE

### 2. Request Configuration
- **URL Input**: Enter any HTTP/HTTPS endpoint
- **Headers Management**: Add custom headers in JSON format
- **Request Body**: Two formats supported:
  - JSON data
  - Form Data (including file uploads)

### 3. Response Visualization
- Status code display
- Response headers viewing
- Formatted response body display (JSON/Text)
- Auto-formatting of JSON responses

### 4. Test Case Management
- Save test cases with custom names
- Load saved test cases
- Delete unwanted test cases
- Export all test cases to JSON file
- Import test cases from JSON file
- Local storage persistence

## How to Use

### Basic Setup
1. Download the `index.html` file
2. Open it in any modern web browser
3. Start testing your APIs immediately

### Making a Request
1. Select the HTTP method (GET, POST, etc.)
2. Enter the API URL
3. Add headers if required (in JSON format)
4. Choose request type:
   - JSON: Enter request body in JSON format
   - Form Data: Add key-value pairs or file uploads
5. Click "Send Request"

### Managing Test Cases
1. **Save a Test Case**:
   - Configure your request
   - Click "Save Test Case"
   - Enter a name for the test case

2. **Load a Test Case**:
   - Click "Show Saved Tests"
   - Click on the desired test case from the sidebar

3. **Export Tests**:
   - Click "Export All Tests"
   - Save the JSON file to your computer

4. **Import Tests**:
   - Click "Import Tests"
   - Select previously exported JSON file

## Example Usage

### Testing a GET Request

URL: https://api.example.com/users
Method: GET
Headers: {
    "Authorization": "Bearer your-token-here"
}

### Testing a POST Request

URL: https://api.example.com/users
Method: POST
Headers: {
    "Content-Type": "application/json"
}
Body: {
    "name": "John Doe",
    "email": "john@example.com"
}

## Technical Details

### Storage
- Uses browser's localStorage for saving test cases
- Data persists between sessions
- Export/Import feature for data backup and sharing

### Security Notes
- Runs entirely in the browser
- No data is sent to any server except the API endpoints you specify
- CORS restrictions apply as per browser security policies

### Browser Compatibility
- Works with all modern browsers:
  - Chrome (recommended)
  - Firefox
  - Safari
  - Edge

## Limitations
1. CORS restrictions may prevent testing some APIs
2. File size limitations for localStorage
3. No environment variables support
4. No automated testing features

## Contributing
Feel free to fork this project and submit pull requests for any improvements you'd like to add. Some areas for potential enhancement:
- Environment variables support
- Request/Response history
- Authentication helpers
- Request timing information
- Cookie management
- GraphQL support

## License
MIT License - feel free to use this tool for any purpose.

## Support
For issues, questions, or suggestions, please open an issue in the GitHub repository.

---
Created with ❤️ for API testing
