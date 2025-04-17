# Swagger API Documentation Hosting

This project provides a simple way to host and view Swagger/OpenAPI documentation for your APIs using Swagger UI.

## Overview

This repository contains:

- HTML files for hosting Swagger UI
- YAML files containing API specifications
- Configuration for displaying API documentation in a browser

## Files

- `notification_service_api.yaml` - OpenAPI specification for the Notification Service API
- `notification_service.html` - HTML file specifically for viewing the Notification Service API
- `notification_api_docs.html` - Alternative HTML viewer with custom styling
- `load_swagger.html` - Generic Swagger UI loader
- `swagger.yaml` - Sample API specification (can be replaced with your own)

## Getting Started

### Viewing the API Documentation

1. Start a local HTTP server:
   ```
   npx http-server -p 8080 --no-cache
   ```

2. Open one of the following URLs in your browser:
   - http://localhost:8080/notification_service.html - Notification Service API documentation
   - http://localhost:8080/notification_api_docs.html - Alternative styled documentation
   - http://localhost:8080/load_swagger.html - Generic Swagger UI

### Customizing the API Documentation

To customize the API documentation:

1. Edit the YAML files to update your API specifications
2. Refresh the browser to see the changes

### Adding a New API

To add a new API:

1. Create a new YAML file with your API specification
2. Create a new HTML file based on the existing templates
3. Update the HTML file to point to your new YAML file

## Troubleshooting

If you encounter issues with the documentation not updating:

1. Clear your browser cache
2. Use the `--no-cache` option when starting the HTTP server
3. Add a cache-busting query parameter to the YAML URL in the HTML file

## Additional Resources

- [Swagger UI Documentation](https://swagger.io/tools/swagger-ui/)
- [OpenAPI Specification](https://swagger.io/specification/)
- [Swagger Editor](https://editor.swagger.io/) - Online editor for OpenAPI specifications
