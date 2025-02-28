# Image Metadata Viewer

A modern web application built with Astro that allows users to upload images, view their metadata, and display location data on a map.

![Image Metadata Viewer App](https://cdnjs.cloudflare.com/ajax/libs/emojione/2.2.7/assets/png/1f4f7.png)

## Features

- **Image Upload**: Drag and drop or file selection
- **Metadata Extraction**: Automatically extracts EXIF data from images
- **Metadata Display**: Shows organized metadata in categories
- **Location Mapping**: Displays GPS coordinates on an interactive map
- **Responsive Design**: Works on desktop and mobile devices

## Technologies Used

- [Astro](https://astro.build/) - Fast, modern web framework
- [Exif.js](https://github.com/exif-js/exif-js) - JavaScript library to extract EXIF metadata
- [Leaflet.js](https://leafletjs.com/) - Interactive maps library
- Modern CSS with custom properties and flexbox/grid layouts

## Installation

### Prerequisites

- Node.js (v16.x or later)
- npm or yarn

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Wisauw/MetaExplorer.git
   cd MetaExplorer
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:4321](http://localhost:4321)

## Build for Production

```bash
npm run build
# or
yarn build
```

The built files will be in the `dist` directory, ready to be deployed to any static hosting service.

## Usage Guide

1. **Upload an Image**:
   - Click the "Select Image" button, or
   - Drag and drop an image onto the upload area

2. **View Image and Metadata**:
   - The uploaded image appears in the left card
   - Metadata is displayed in the right card, organized by categories

3. **View Location (if available)**:
   - If the image contains GPS coordinates, a map will appear below showing the location

## Metadata Categories

The app organizes metadata into the following categories:

- **Basic**: Camera make/model, date taken, etc.
- **Camera**: Exposure details, ISO, aperture, etc.
- **Image**: Image dimensions, resolution, orientation
- **Location**: GPS coordinates and related data
- **Other**: Any additional metadata

## Troubleshooting

- **No metadata appears**: Some images (especially screenshots or web images) don't contain EXIF metadata
- **No map appears**: The image doesn't contain GPS location data
- **Map doesn't load properly**: Check your internet connection (needed for map tiles)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Exif.js for the metadata extraction library
- Leaflet.js for the mapping functionality
- OpenStreetMap for providing the map tiles
