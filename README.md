# Discogs Collection Viewer

A modern web application that allows you to view and search through your Discogs vinyl collection. Built with React, TypeScript, and Vite.

## Features

- 🔍 **Search by Artist**: Filter your collection by artist name in real-time
- 📱 **Responsive Design**: Works perfectly on desktop and mobile devices
- 🎨 **Modern UI**: Beautiful gradient design with smooth animations
- ⚡ **Fast Loading**: Efficient pagination and caching
- 🔄 **Real-time Filtering**: Instant search results as you type

## Getting Started

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn

### Installation

1. Clone or download this repository
2. Navigate to the project directory
3. Install dependencies:

```bash
npm install
```

### Running the Application

Start the development server:

```bash
npm run dev
```

The application will open automatically in your browser at `http://localhost:3000`.

### Building for Production

To create a production build:

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## How to Use

1. **Enter Your Username**: When the app loads, enter your Discogs username in the form
2. **View Your Collection**: The app will fetch and display all records in your collection
3. **Search Records**: Use the search bar at the top to filter records by artist name
4. **Browse Records**: Click on any record card to see more details (future feature)

## API Information

This application uses the Discogs API to fetch user collections. The API has rate limits:

- **Public API**: Limited to 60 requests per minute
- **Authenticated API**: Higher limits available with API key

For production use, consider:
- Obtaining a Discogs API key for higher rate limits
- Implementing proper caching mechanisms
- Adding error handling for network issues

## Technical Details

### Tech Stack

- **Frontend**: React 18 with TypeScript
- **Build Tool**: Vite
- **Styling**: CSS with modern features (Grid, Flexbox, CSS Variables)
- **HTTP Client**: Axios
- **API**: Discogs REST API

### Project Structure

```
src/
├── components/          # React components
│   ├── UsernameForm.tsx
│   ├── SearchBar.tsx
│   └── RecordCard.tsx
├── services/           # API services
│   └── discogsApi.ts
├── types.ts           # TypeScript type definitions
├── App.tsx           # Main application component
├── main.tsx          # Application entry point
└── index.css         # Global styles
```

### Key Features Implementation

- **Pagination**: Automatically fetches all pages of the user's collection
- **Search**: Client-side filtering for instant results
- **Error Handling**: Comprehensive error messages for various scenarios
- **Loading States**: Smooth loading indicators and transitions
- **Responsive Design**: Mobile-first approach with CSS Grid

## Troubleshooting

### Common Issues

1. **"User not found" error**: Double-check the Discogs username spelling
2. **Rate limit errors**: Wait a minute and try again, or use an API key
3. **No records displayed**: Ensure the user has a public collection

### Rate Limiting

The Discogs API has rate limits. If you encounter rate limit errors:
- Wait 60 seconds before trying again
- Consider implementing a proper API key for higher limits
- The app will show appropriate error messages

## Contributing

Feel free to contribute to this project by:
- Reporting bugs
- Suggesting new features
- Submitting pull requests

## License

This project is open source and available under the MIT License.

## Acknowledgments

- [Discogs API](https://www.discogs.com/developers/) for providing the data
- [React](https://reactjs.org/) for the frontend framework
- [Vite](https://vitejs.dev/) for the build tool #
