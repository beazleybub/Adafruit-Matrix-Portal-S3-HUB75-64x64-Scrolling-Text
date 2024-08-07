Adafruit MatrixPortal S3 64x64 HUB75 Scrolling Text Display

This project demonstrates how to display two lines of scrolling text on a 64x64 HUB75 LED matrix using the Adafruit MatrixPortal S3.

## Features
- Two lines of smoothly scrolling text.
- Designed for a 64x64 HUB75 LED matrix.
- Utilizes the Adafruit MatrixPortal S3.

## Getting Started

### Prerequisites
- Adafruit MatrixPortal S3
- 64x64 HUB75 LED matrix
- Appropriate power supply for your LED matrix
- USB cable for programming the MatrixPortal S3

### Hardware Setup
1. Connect your 64x64 HUB75 LED matrix to the Adafruit MatrixPortal S3.
2. Ensure the power supply is connected to the LED matrix.
3. Connect the MatrixPortal S3 to your computer using a USB cable.

### Software Setup

1. **Install CircuitPython on Your MatrixPortal S3**:
   - Download the latest CircuitPython firmware for the MatrixPortal S3 from [Adafruit's CircuitPython Downloads](https://circuitpython.org/board/adafruit_matrixportal_s3/).
   - Follow the instructions on the download page to flash CircuitPython onto your MatrixPortal S3.

2. **Install the CircuitPython Libraries**:
   - Download the latest version of the Adafruit CircuitPython Bundle from [CircuitPython Libraries](https://circuitpython.org/libraries).
   - Extract the downloaded zip file.
   - Copy the necessary libraries from the extracted bundle to the `lib` directory on your MatrixPortal S3's CIRCUITPY drive. The required libraries for this project are:
     - `adafruit_display_text`
     - `adafruit_rgb_matrix`
     - `adafruit_framebufferio`

3. **Copy the Project Code**:
   - Copy the `code.py` file from this repository to the root of your CIRCUITPY drive.

### Usage
- Once the code is uploaded, the MatrixPortal S3 will start displaying the scrolling text on the LED matrix.

## Customization
### Changing the Text
You can customize the text to be displayed by modifying the following lines in the `code.py` file:

```python
line1 = adafruit_display_text.label.Label(
    terminalio.FONT,
    color=0xff0000,
    text="Your text here for line 1"
)
line2 = adafruit_display_text.label.Label(
    terminalio.FONT,
    color=0x0080ff,
    text="Your text here for line 2"
)
```

### Adjusting the Scroll Speed
To change the scrolling speed, adjust the delay in the main loop of the `code.py` file:

```python
time.sleep(0.05)  # Adjust the sleep time to slow down or speed up the scrolling
```

## Troubleshooting
- Ensure all connections are secure and correctly placed.
- Verify that you have installed all the required libraries.
- Check the power supply to ensure it is adequate for your LED matrix.

## Contributing
If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Contributions are welcome!

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements
- [Adafruit](https://www.adafruit.com/) for their excellent hardware and libraries.
- The open-source community for their contributions and support.

---

This README should guide users on how to set up and use your project effectively. If you have any other questions or need further assistance, feel free to ask!
