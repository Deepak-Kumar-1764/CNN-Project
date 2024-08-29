# Dog and Cat Classifier with Deep Learning

This project is a web application developed using Flask and TensorFlow that leverages deep learning for classifying images as either dogs or cats using a pre-trained convolutional neural network (CNN) model.


## Features

- **Image Classification**: Classify uploaded images as either "Dog" or "Cat".
- **User Interface**: Simple web interface allowing users to upload images and view classification results.
- **Error Handling**: Displays appropriate messages when no file is uploaded.

## Project Structure

- **`app.py`**: The main Flask application file that handles routing, image processing, and model prediction.
- **`templates/home.html`**: The home page template where users upload their images.
- **`templates/classify.html`**: The results page that displays the classification result and image.
- **`static/styles.css`**: Custom CSS for styling the application.
- **`static/images/`**: Directory containing images used for the background of the web pages.
- **`static/models/dog_cat_M.h5`**: The pre-trained TensorFlow model for image classification.
- **`uploads/`**: Directory where uploaded images are temporarily stored.

## Installation

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/Deepak-Kumar-1764/dog-cat-classifier.git
    cd dog-cat-classifier
    ```

2. **Create a Virtual Environment**:

    ```bash
    python -m venv venv
    ```

3. **Activate the Virtual Environment**:

    - On Windows:

        ```bash
        venv\Scripts\activate
        ```

    - On macOS/Linux:

        ```bash
        source venv/bin/activate
        ```

4. **Install Dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

5. **Download the Pre-Trained Model**:
   Ensure that the pre-trained TensorFlow model `dog_cat_M.h5` is placed in the `static/models/` directory. You can find this model from the project's provided sources or pre-trained models repository.

6. **Run the Application**:

    ```bash
    python app.py
    ```

7. **Access the Application**:
   Open a web browser and navigate to `http://127.0.0.1:5000/` to use the application.

## Code Overview

- **`app.py`**: 
    - Loads the TensorFlow model.
    - Defines routes for the home page and image classification.
    - Handles file uploads and image classification logic.
    - Displays error messages if no file is uploaded.

- **`home.html`**:
    - Provides the form for image upload.
    - Displays error messages if no image is uploaded.

- **`classify.html`**:
    - Shows the uploaded image and classification results.
    - Provides a button to return to the home page.

- **`styles.css`**:
    - Contains custom styles for the application.

## Error Handling

- If no image is uploaded, the application will display a message asking the user to upload an image.
- If the upload folder does not exist, it will be created to prevent errors.

## Contribution

Feel free to fork the repository and contribute by submitting pull requests or opening issues.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
