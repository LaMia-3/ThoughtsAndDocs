# Book Collection App

## Description
Book Collection App is a modern web application for tracking and managing your personal book collection. It provides a beautiful, intuitive interface for users to catalog their books, track reading progress, organize books into series and collections, and visualize reading habits through detailed insights. The app features offline support through IndexedDB storage, multiple view options (bookshelf, list, and cover grid), and integration with book APIs for easy addition of new books.

## Goals
- Create a beautiful, intuitive interface for managing personal book collections
- Provide multiple ways to view and organize books (shelf, list, cover grid)
- Support offline usage with local data storage
- Enable tracking of reading progress and completion dates
- Facilitate organization of books into series and custom collections
- Offer insights and statistics about reading habits
- Allow import/export of book data for backup and portability
- Implement customization options for personalized experience

## Current Status
- Status: In Progress
- Started: November 2025
- Last Updated: February 16, 2026

## Features

### Core Features
- **Book Management**
  - Add books via Google Books API or Open Library API
  - Track reading status (Want to Read, Reading, Completed, On Hold, DNF)
  - Edit book details (title, author, page count, descriptions, genres)
  - Organize books into series with automatic detection

### Views
- **Bookshelf View**: Visual representation of books as spines on shelves
- **List View**: Detailed list with sorting and filtering options
- **Cover Grid**: Visual browsing of book covers
- **Insights**: Dashboard with reading statistics and visualizations

### Organization
- **Series Management**: Group books into series with reading order
- **Collections**: Create custom collections for organizing books by theme, project, or any criteria
- **Tags**: Apply and filter by custom tags

### Data Management
- **Offline Support**: Full functionality without internet connection
- **Import/Export**: CSV and JSON formats for data portability
- **Database Repair**: Tools for troubleshooting and fixing database issues

## Technology Stack
- **Frontend**: React 18 with TypeScript 5
- **UI Components**: shadcn/ui with Tailwind CSS
- **Storage**: IndexedDB with localStorage for UI preferences
- **Build Tool**: Vite 5.x
- **Deployment**: Vercel for continuous deployment and hosting
- **External APIs**: Google Books API, Open Library API

## Roadmap
- [x] Core book management functionality
- [x] Multiple view options (shelf, list, cover)
- [x] Series organization
- [x] Collections feature
- [x] Import/Export functionality
- [x] Reading goals tracking
- [x] Database troubleshooting tools
- [ ] Enhanced statistics and insights
- [ ] Cloud sync option (using MongoDB Atlas)
- [ ] Social sharing features

## Notes
- The app uses a hybrid storage approach with IndexedDB as the primary data store
- UI preferences and some settings are stored in localStorage for quick access
- The app is designed to work completely offline
- Performance optimizations include virtualization for large collections

## Resources
- [Deployed App](https://book-collection-app-blue.vercel.app/)
- [GitHub Repository](https://github.com/LaMia-3/book-collection-app)
- [Google Books API](https://developers.google.com/books)
- [Open Library API](https://openlibrary.org/developers/api)
- [shadcn/ui Documentation](https://ui.shadcn.com)
- [IndexedDB Documentation](https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API)

## Tags
#project #react #typescript #books #reading #personal-library #offline-app
