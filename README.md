# Virtual-Background-Replacement
# Background Replacement using OpenCV in Google Colab

This project performs simple background replacement for an uploaded image using OpenCV. It separates the foreground using basic grayscale thresholding and overlays it on a new virtual background.

## Features

- Upload input and background images via Colab.
- Automatically resizes background to match input dimensions.
- Applies grayscale thresholding to extract the foreground.
- Combines the extracted foreground with a virtual background.
- Saves and displays the final output image.

## Requirements

This notebook runs in [Google Colab](https://colab.research.google.com/) and uses the following Python libraries:

- `cv2` (OpenCV)
- `numpy`
- `google.colab` for file upload and image display

No installation is required in Colab as all dependencies come pre-installed.

## Usage

1. **Open the notebook in Google Colab.**
2. **Run the first cell to upload your images**:
   - Upload one image for the subject.
   - Upload another image to be used as the virtual background.
3. **Set the file paths** in the script (or modify to auto-detect from `uploaded.keys()`).
4. **Run the processing cells**.
5. The output image will be displayed and saved as `output_image_alternate.jpg`.

## Example

```python
input_image_path = "/content/your_subject.jpg"
virtual_bg_path = "/content/your_background.jpg"
