# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Django 5.2.4 project named "d_n_s" with plans for authentication and feature showcase functionality. The project structure includes:

- **Virtual Environment**: `DNS_env/` (Python virtual environment)
- **Django Project**: `d_n_s/` (main project directory)
- **Project Configuration**: `d_n_s/d_n_s/` (Django settings, URLs, WSGI/ASGI)

## Common Commands

### Environment Setup
```bash
# Activate virtual environment (Windows)
DNS_env\Scripts\activate

# Activate virtual environment (Linux/Mac)
source DNS_env/bin/activate
```

### Development Commands
```bash
# Run development server
python d_n_s/manage.py runserver

# Create database migrations
python d_n_s/manage.py makemigrations

# Apply migrations
python d_n_s/manage.py migrate

# Create superuser
python d_n_s/manage.py createsuperuser

# Create new Django app
python d_n_s/manage.py startapp <app_name>
```

## Architecture

### Current Structure
- **Django Project**: `d_n_s/d_n_s/` - Contains main project configuration
  - `settings.py` - Django settings (uses SQLite database, development mode)
  - `urls.py` - URL routing (currently only admin URLs)
  - `wsgi.py` / `asgi.py` - Server configurations

### Planned Applications
According to the project prompt, two Django apps are planned:
1. **authentication** - For login, logout, and registration functionality
2. **home_page** - Main dashboard with feature showcase flow

### Feature Showcase Flow
The project is designed to have a progressive feature demonstration:
1. User completes authentication
2. Navigates to home_page app
3. Views features one by one with smooth transitions
4. Finally reaches the main dashboard

## Development Notes

- Uses Django 5.2.4
- SQLite database (default Django setup)
- Debug mode enabled (development settings)
- Secret key is in settings.py (development only - should be moved to environment variables for production)
- All Django files are located in the `d_n_s/` subdirectory
- Virtual environment is named `DNS_env`

## Working Directory

When working on this project, navigate to the `d_n_s/` directory for Django management commands, as the `manage.py` file is located there.