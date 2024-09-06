# Character-Level-Text-Generation-Using-LSTM-on-Shakespeare

## Overview
This project utilizes LSTM networks to generate text at the character level, trained on Shakespeare's works. The model predicts the next character in sequences, enabling the creation of text mimicking Shakespeare's style with adjustable creativity.



## Features

- **Text Data**: Uses Shakespeare's text data available from TensorFlow's dataset repository.
- **Data Preparation**: Processes the text into sequences for training the LSTM model.
- **Model Architecture**: Utilizes an LSTM-based neural network with a softmax output layer.
- **Text Generation**: Generates text based on different temperature settings to control the creativity of the output.

## Getting Started

To get started with this project, follow these steps:

### 1. Clone the Repository

```bash
git clone https://github.com/varsityyy/Character-Level-Text-Generation-Using-LSTM-on-Shakespeare.git
```



### 2. Navigate to the Project Directory

```bash
cd repository
```

### 3. Install Dependencies

Ensure you have Python installed. Then, install the required packages using `pip`:

```bash
pip install tensorflow numpy
```

### 4. Run the Script

Execute the Python script to train the model and generate text:

```bash
python generate_text.py
```

The script will output generated text samples with different temperature settings.

## Project Structure

- `generate_text.py`: The main script containing the LSTM model training and text generation code.
- `README.md`: This file.
- `requirements.txt`: List of Python packages required for the project (auto-generated).

## Code Explanation

1. **Data Preparation**: 
   - Fetches Shakespeare's text and preprocesses it into sequences of characters.
   - Creates one-hot encoded input sequences and target outputs.

2. **Model Definition**: 
   - Defines an LSTM model with 128 units and a Dense layer with a softmax activation function.

3. **Training**: 
   - Compiles the model using categorical cross-entropy loss and RMSprop optimizer.
   - Trains the model on the preprocessed text data.

4. **Text Generation**: 
   - Defines a function to sample from the model's predictions and generate text based on the given temperature.

## Example Output

The script generates text samples with different temperature settings (0.2 to 0.8). Lower temperatures result in more predictable text, while higher temperatures produce more varied and creative outputs.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- TensorFlow for providing the LSTM implementation.
- NumPy for numerical operations.

## Contact

For any questions or feedback, please open an issue on the [GitHub repository](https://github.com/varsityyy/Character-Level-Text-Generation-Using-LSTM-on-Shakespeare).

---
