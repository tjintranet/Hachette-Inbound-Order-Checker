# Order Processing Tool

## Overview
A web-based application designed to process and display order information from text files. The tool provides a simple interface for uploading order files, displaying the data in a tabular format, and exporting the results to CSV.

## Features
- File upload interface for order text files
- Table display showing:
  - Date (DD/MM/YYYY format)
  - Order Number
  - Total Copies
- Automatic calculation of total copies per order
- Grand total calculation displayed in the footer
- Export functionality to CSV
- Clear All function to reset the display
- Responsive design that works on both desktop and mobile devices

## Technical Requirements
- Modern web browser with JavaScript enabled
- No server-side requirements (runs entirely in the browser)
- Internet connection for loading CDN resources:
  - Bootstrap 5.3.2
  - Bootstrap Icons
  - Font Awesome 6.4.0

## File Structure
```
├── index.html      # Main application file
├── favicon-32x32.png   # Favicon image
└── apple-touch-icon.png # Apple touch icon
```

## Input File Format
The tool expects a text file with the following format:
- H1 lines containing order number and date
- D1 lines containing order details and quantities
Example:
```
H17000681599     20250128
D17000681599     7844445-21               00001   0000010000000000000000000000
```

## Installation
1. Download all files to a local directory
2. Open `index.html` in a web browser
   - No additional installation or setup required
   - Can be hosted on any web server

## Usage Instructions
1. Open the application in a web browser
2. Click "Choose File" to select an order text file
3. The data will automatically be processed and displayed
4. Use the "Download CSV" button to export the data
5. Use "Clear All" to reset the application

## CSV Export Format
The exported CSV file includes:
- Headers: Date, Order Number, Total Copies
- Data rows with corresponding values
- Footer row with total copies (shifted one column right)

## Browser Compatibility
Tested and compatible with:
- Google Chrome (latest)
- Mozilla Firefox (latest)
- Microsoft Edge (latest)
- Safari (latest)

## Known Limitations
- Processes one file at a time
- Limited to text file format specified above
- Requires JavaScript to be enabled

## Error Handling
The application includes error handling for:
- Invalid file formats
- File reading errors
- Data processing errors
- All errors are displayed to the user in the interface

## Performance
- Designed to handle files with hundreds of orders
- Client-side processing for immediate results
- Minimal memory footprint

## Security
- All processing done client-side
- No data transmitted to any server
- No data stored between sessions

## Support and Maintenance
For support or to report issues:
1. Check browser console for error messages
2. Verify file format matches expected input
3. Clear browser cache if experiencing issues
4. Contact system administrator for additional support

## Future Enhancements
Potential improvements could include:
- Batch file processing
- Additional export formats
- Data filtering and sorting
- Customizable date formats
- Search functionality

## Version History
- 1.0.0 - Initial release with basic functionality
  - File upload
  - Table display
  - CSV export
  - Total calculations