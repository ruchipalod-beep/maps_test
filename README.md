# Custom Map Layers for Analytics Reporting

This repository contains custom map layers for analytics reporting, allowing you to create and use custom geographic visualizations beyond the built-in Looker map layers.

## Overview

This tool enables the generation of custom map layers for reporting purposes. Instead of relying solely on built-in Looker map layers, you can now create your own custom geographic visualizations using GeoJSON files.

## Prerequisites

- Access to [geojson.io](https://geojson.io) (powered by Mapbox)
- Access to internal map layers repository
- Looker reporting access

## How to Create Custom Map Layers

### Step 1: Create GeoJSON File

1. Visit [geojson.io](https://geojson.io) (powered by Mapbox)
2. Use the drawing tools to **select the area of interest** (options highlighted in red)
3. Click **Save** and download the JSON file

### Step 2: Upload to Repository

1. Upload the downloaded JSON file to the map layers folder in our internal repository
2. Ensure the file is properly named and organized

### Step 3: Use in Reports

1. Navigate to the JSON file in the internal repository
2. Click **Raw** (highlighted in red)
3. Copy the URL of the raw file
4. In your Looker visualization:
   - Go to **Visualization** settings
   - Select **Custom** option
   - Paste the raw file URL

## File Structure

```
maps_test/
├── map_layer/
│   ├── africa.json          # Africa map layer
│   └── india-states.json    # India states map layer
├── README.md                # This documentation
└── Read ME - GeoJson.docx   # Original instructions
```

## Available Map Layers

- **Africa**: Complete African continent map layer
- **India States**: Indian states and territories map layer

## Adding New Map Layers

To add new custom map layers:

1. Create your GeoJSON file using geojson.io
2. Save it in the `map_layer/` directory
3. Update this README with the new layer information
4. Follow the usage instructions above to implement in reports

## Technical Notes

- All map layers are stored as GeoJSON files
- Files should be optimized for web performance
- Coordinate reference numbers may be included for specific geographic areas

## Support

For questions or issues with custom map layers, please refer to the internal documentation or contact the analytics team.

## External Resources

- [GeoJSON.io](https://geojson.io) - Online GeoJSON editor
- [Mapbox](https://mapbox.com) - Mapping platform
- [GeoJSON Specification](https://geojson.org/) - Official GeoJSON format documentation