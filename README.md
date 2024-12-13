# Steganography Project

## Overview
Steganography is the practice of concealing messages or information within other non-secret text or data. This project demonstrates a simple steganography application that allows users to hide secret messages inside image files and later extract them securely.

---

## Features

- **Embed Secret Messages:** Hide text messages inside image files using an efficient encoding algorithm.
- **Extract Messages:** Retrieve the hidden text from the encoded image.
- **Supported Formats:** Works with popular image formats such as PNG and BMP.
- **Password Protection:** Add an optional password for securing the hidden message.
- **User-Friendly Interface:** Simple GUI or command-line options for easy interaction.

---

## Technologies Used

- **Programming Language:** Python
- **Libraries:**
  - `Pillow`: For image manipulation
  - `Tkinter` (Optional): For GUI-based interaction
  - `argparse`: For command-line usage

---

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/steganography-project.git
   cd steganography-project
   ```

2. **Install Dependencies:**
   Make sure Python 3.x is installed. Then run:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### Command Line Interface

- **Embed a Message:**
  ```bash
  python steganography.py embed --image input_image.png --message "Your secret message" --output output_image.png
  ```

- **Extract a Message:**
  ```bash
  python steganography.py extract --image output_image.png
  ```

- **With Password Protection:**
  ```bash
  python steganography.py embed --image input_image.png --message "Your secret message" --output output_image.png --password mypassword
  python steganography.py extract --image output_image.png --password mypassword
  ```

### GUI Interface (Optional)
Run the following command to launch the GUI:
```bash
python gui_steganography.py
```

---

## Examples

### Embedding a Secret Message
Input Image:
![Input Image](images/input_image_example.png)

Output Image:
![Output Image](images/output_image_example.png)

### Extracting the Message
The hidden message is revealed using the extraction tool:
```
Secret Message: "Hello, World!"
```

---

## Limitations

- The size of the secret message is limited by the dimensions of the image.
- Excessive modification of the encoded image might corrupt the hidden message.

---

## Contributing

Contributions are welcome! Feel free to fork this repository and submit a pull request with your improvements.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For any inquiries or support, please contact:

- **Name:** Your Name
- **Email:** your.email@example.com
- **GitHub:** [Your GitHub Profile](https://github.com/yourusername)

---

Happy Steganography! 😊

