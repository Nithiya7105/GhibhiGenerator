# GhibhiGenerator by NithiyaShri

**GhibhiGenerator** is a Gradio-powered web application that transforms user-uploaded images into anime-style artwork inspired by Studio Ghibli and other anime aesthetics. It uses the `AtelierGenerator` engine with integrated LoRA models to produce high-quality stylistic variations.

---

## Features

* Upload and transform images into anime-inspired styles
* Uses multiple fine-tuned LoRA models:

  * Studio Ghibli
  * Anime Plus
  * SoftServe Anime
* Caches image captions to reduce processing time on repeated inputs
* Custom UI styling with Gradio and CSS for improved user experience

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Nithiya7105/GhibhiGenerator.git
   cd GhibhiGenerator
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:

   ```bash
   python app.py
   ```

This will launch the GhibhiGenerator interface in your default web browser.

---

## File Overview

```plaintext
GhibhiGenerator/
│
├── app.py               # Main application file
├── requirements.txt     # Dependency list
└── README.md            # Project documentation
```

---

## How It Works

1. The user uploads an image through the interface.
2. The application generates a caption for the image using `AtelierGenerator` (or retrieves it from cache if previously processed).
3. Based on the selected LoRA style, the application generates a variation of the uploaded image.
4. The result is displayed in a gallery for the user.

---

## Supported Styles

| Style Name    | LoRA Model Path             |
| ------------- | --------------------------- |
| Studio Ghibli | NithiyaShri/studio-ghibli   |
| Anime Plus    | NithiyaShri/anime-plus      |
| SoftServe     | NithiyaShri/softserve-anime |

---

## Disclaimer

This project is developed for personal and educational use. Image generation may take longer than expected due to high demand or computational limits. Ensure you have the appropriate permissions to use any uploaded content.

All rights reserved © 2025 NithiyaShri.

---

## License

This repository is provided without any license file. By default, all rights are reserved to the author unless otherwise specified.

