# Product Image Search (ML Kit Edition)

An Android application that implements **Google's ML Kit Object Detection API** to identify products in images and prepare them for a visual search experience.

## 🚀 Features

- **Real-time Object Detection**: Identifies multiple objects within an image using ML Kit.
- **Fashion Item Specialization**: Specifically tuned to detect fashion-related goods.
- **Interactive UI**: Users can tap on detected objects to select and crop them.
- **Visual search**: Integrated with a Vision Product Search API to find similar products in real-time.
- **Search Results Screen**: A dedicated activity to display matched items, similarity scores, and product metadata.
- **Multiple Image Sources**:
    - **Camera**: Capture new photos directly within the app.
    - **Gallery**: Select existing images from the device storage.
    - **Presets**: Quick-start with high-quality sample images from the assets folder.
- **Dynamic Image Processing**: Handles UI scaling and aspect ratios to ensure accurate detection mapping on all screen sizes.

## 🛠️ Technical Stack

- **Language**: Kotlin
- **ML Framework**: [Google ML Kit (Object Detection & Tracking)](https://developers.google.com/ml-kit/vision/object-detection)
- **Image Loading**: [Glide](https://github.com/bumptech/glide) for efficient image handling and caching.
- **UI Components**: 
    - Material Design Components.
    - Custom `ImageClickableView` for interactive detection overlays.
- **Networking**: [Volley](https://github.com/google/volley) for API integrations.
- **Data Handling**: [Gson](https://github.com/google/gson) for JSON parsing.

## 📁 Project Structure

- **`ObjectDetectorActivity.kt`**: The main entry point that manages the camera/gallery intents and runs the ML Kit processing loop.
- **`ProductSearchActivity.kt`**: Handles the display and interaction with visual search results.
- **`ProductSearchAPIClient.kt`**: Manages the network requests to the Vision Product Search backend.
- **`ImageClickableView.kt`**: A custom view that overlays detection "dots" on the image and handles tap-to-crop functionality.

## 🚧 Status

- **Version 1.0**: Core features and search implementation fully integrated.

---
*Created as part of the Google Codelabs series on Machine Learning.*

