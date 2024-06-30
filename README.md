# POKEMON IMAGE CLASSIFICATION

This project classifies images of Pokémon (Pikachu, Bulbasaur, Charmander) using a Convolutional Neural Network (CNN).

## Dataset

The dataset consists of images divided into training and test sets:
- **Train Data**: Contains images of Pokémon in separate folders for each class.
- **Test Data**: Contains images for testing the model.

## Model

The model is a Sequential CNN with the following layers:
- **Convolutional Layers**: Extract features from images.
- **MaxPooling Layers**: Reduce spatial dimensions.
- **Flatten Layer**: Flatten the input.
- **Dense Layer**: Output layer with softmax activation.

### Architecture
- **Conv2D**: 32 filters, (3,3) kernel, ReLU activation
- **Conv2D**: 64 filters, (3,3) kernel, ReLU activation
- **MaxPooling2D**
- **Conv2D**: 128 filters, (3,3) kernel, ReLU activation
- **MaxPooling2D**
- **Flatten**
- **Dense**: 3 units, softmax activation

## Training

The model is trained using the Adam optimizer and categorical cross-entropy loss function. The training data is augmented to improve model generalization.

## Evaluation

The model's performance is evaluated on a test set, achieving an accuracy of approximately 97%.

## Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/DevanshChhabra/POKEMON-IMAGE-CLASSIFICATION.git
    cd POKEMON-IMAGE-CLASSIFICATION
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Train the model**:
    ```python
    python train.py
    ```

4. **Evaluate the model**:
    ```python
    python evaluate.py
    ```

## Results

- The model correctly classifies Pokémon images with high accuracy.
- Sample predictions:
    - Charmander: Correct
    - Pikachu: Correct

## Acknowledgments

This project showcases CNN capabilities in image classification, inspired by a love for Pokémon.

## License

This project is licensed under the MIT License.
