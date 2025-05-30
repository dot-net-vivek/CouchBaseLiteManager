# CouchBase DB Editor

A modern, intuitive Windows application for managing CouchBase Lite databases with a beautiful Blazor Hybrid interface.

## 🚀 Features

- **Database Management**: Create, open, and manage CouchBase Lite databases
- **Visual Database Explorer**: Browse database contents with an intuitive two-panel interface
- **Schema-Based Forms**: Define object schemas for dynamic form generation
- **Document Operations**: Full CRUD operations (Create, Read, Update, Delete) for documents
- **Advanced Querying**: Support for both simple search and N1QL (CouchBase SQL) queries
- **Query Preview**: Preview query results before executing full queries
- **Pagination**: Efficient handling of large datasets with pagination
- **Toast Notifications**: Real-time feedback for all operations
- **Modern UI**: Responsive design built with Bootstrap 5 and Bootstrap Icons
- **Type Safety**: Automatic type conversion and validation for form fields

## 📋 System Requirements

### Required Dependencies
- **Operating System**: Windows 10 (version 1909 or later) or Windows 11
- **.NET 8.0 Runtime**: Download from [Microsoft .NET Downloads](https://dotnet.microsoft.com/download/dotnet/8.0)
- **Microsoft Edge WebView2**: Usually pre-installed on Windows 11 and recent Windows 10 updates
  - If needed, download from [WebView2 Downloads](https://developer.microsoft.com/microsoft-edge/webview2/)

### Hardware Requirements
- **RAM**: Minimum 4GB (8GB recommended)
- **Storage**: 100MB free disk space for application + space for databases
- **Processor**: Any modern Intel/AMD processor
- **Display**: 1024x768 minimum resolution (1920x1080 recommended)

### Compatibility Notes
- **WebView2**: Comes pre-installed on Windows 11 and most Windows 10 systems with recent updates
- **Admin Rights**: Not required for running the application
- **Network**: Not required (offline-capable application)

## 📦 Installation

### Option 1: Using the Installer (Recommended)
1. Download the latest installer from the [Releases](../../releases) page
2. Run `CouchBaseDBEditor-Setup.exe`
3. Follow the installation wizard
4. The installer will check for dependencies and guide you through any required downloads

### Option 2: Manual Installation
1. Ensure .NET 8.0 Runtime is installed
2. Ensure WebView2 is available (usually pre-installed)
3. Download and extract the application files
4. Run `CouchBaseDBEditor.exe`

## 📖 Usage Guide

### Getting Started
1. **Launch the Application**: Run CouchBaseDBEditor.exe
2. **Create a Database**: Use the Database menu → Create New Database
3. **Open Existing Database**: Use the Database menu → Open Existing Database
4. **Explore Data**: Navigate to Database Explorer to view and manage your data

### Database Operations
- **Create Database**: Choose directory and enter database name
- **Open Database**: Browse to existing database directory
- **Close Database**: Use Database menu → Close Database

### Managing Objects (Collections)
1. Click **"Add Object"** in the left panel
2. Define object name, description, and type
3. Optionally create a schema with field definitions
4. Choose whether to create sample data

### Adding Data
- **With Schema**: Use the dynamic form generated from your object schema
- **Without Schema**: Enter data in JSON format
- **Required Fields**: Marked with red asterisk (*)

### Querying Data
- **Simple Search**: Use the search box for basic text searches
- **Advanced Queries**: Click "Query" button for N1QL SQL queries
- **Query Preview**: Preview results before executing full query
- **Query Examples**: Built-in examples for common query patterns

### Document Management
- **Edit**: Click the pencil icon next to any document
- **Delete**: Click the trash icon (with confirmation dialog)
- **View Details**: All document fields displayed in the data table

## 🏗️ Architecture

### Technology Stack
- **Frontend**: Blazor Hybrid Components with Microsoft Edge WebView2
- **Backend**: .NET 8.0 Windows Forms application
- **Database**: CouchBase Lite 3.2.3
- **UI Framework**: Bootstrap 5 with Bootstrap Icons
- **Dependency Injection**: Microsoft.Extensions.Hosting


## 🔧 Configuration

### Database Storage
- Databases are stored in user-specified directories
- No special configuration required
- Supports multiple databases (one open at a time)

### Application Settings
- No configuration file required
- All settings managed through the UI
- Schema definitions stored with database metadata

## 🐛 Troubleshooting

### Common Issues

**Application Won't Start**
- Verify .NET 8.0 Runtime is installed
- Check if WebView2 is available
- Run as administrator if permission issues occur

**Database Won't Open**
- Verify database directory exists and is accessible
- Check file permissions on the database directory
- Ensure database name is correct

**Query Errors**
- Use Query Help for syntax examples
- Test with simple search terms before complex N1QL
- Check field names for typos
- Use query preview to validate logic

**Performance Issues**
- Use WHERE clauses to filter large datasets
- Limit SELECT field lists instead of using SELECT *
- Close unused databases to free memory

### Getting Help
- Check the built-in **User Manual** (accessible from the application)
- Review **Query Help** for N1QL syntax examples
- Use browser console (F12) for detailed error logging
- Check application toast notifications for specific error messages

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

### Open Source Components
- **CouchBase Lite** - Database engine (CouchBase License)
- **Bootstrap** - UI framework (MIT License)
- **Bootstrap Icons** - Icon library (MIT License)
- **.NET** - Application framework (MIT License)
- **WebView2** - Web rendering engine (Microsoft License)

## 👨‍💻 Author

Created with ❤️ by [Vivek Gupta](https://www.linkedin.com/in/vivekguptadotnet/)

## 🔄 Version History

### v1.0.0 (Current)
- Initial release
- Complete database management functionality
- Schema-based dynamic forms
- Advanced querying with preview
- Modern Blazor Hybrid UI
- Comprehensive documentation

## 🚀 Future Enhancements

- Multi-database support (multiple open databases)
- Database synchronization with CouchBase Server
- Import/Export functionality
- Database backup and restore
- Advanced schema validation
- Custom query templates
- Dark mode theme

---

**Note**: This application requires Windows 10/11 and is built specifically for the Windows platform using Blazor Hybrid technology for optimal performance and user experience. 
