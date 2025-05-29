<h1>Assignment 1: MNIST Digit Classification with TensorFlow/Keras</h1>

  <p>
    This project was completed as part of the MSDS458-DL: Artificial Intelligence and Deep Learning course at Northwestern University.
    The assignment involved developing and evaluating multiple neural network architectures using TensorFlow/Keras to classify handwritten digits from the MNIST dataset.
  </p>

  <h2>Overview</h2>
  <p>
    The assignment includes an in-depth exploration of various fully connected neural network (FCNN) architectures trained on the MNIST dataset.
    Several architectural variants are tested across multiple notebooks, including:
  </p>
  <ul>
    <li>Varying numbers of hidden layers and neurons</li>
    <li>Different activation functions (e.g., ReLU, tanh)</li>
    <li>Model complexity vs. generalization tradeoffs</li>
    <li>Baseline comparison using Random Forests</li>
  </ul>

  <h2>Dataset</h2>
  <ul>
    <li><strong>MNIST</strong>: 70,000 grayscale images of handwritten digits (0–9), each 28×28 pixels</li>
    <li>Split into 60,000 training and 10,000 test images</li>
    <li>Labels one-hot encoded for use with softmax output layers</li>
  </ul>

  <h2>Key Libraries Used</h2>
  <ul>
    <li>numpy, pandas</li>
    <li>matplotlib, seaborn</li>
    <li>scikit-learn (for PCA, t-SNE, and Random Forests)</li>
    <li>tensorflow (keras)</li>
  </ul>

  <h2>Requirements</h2>
  <p>Designed to run in <strong>Google Colab</strong>, which includes all required libraries.</p>
  <p>If running locally, install:</p>
  <pre><code>pip install numpy pandas matplotlib seaborn scikit-learn tensorflow</code></pre>

  <h2>How to Run</h2>
  <ol>
    <li>Visit the <a href="https://github.com/betzmosk/Deep-Learning-MSDS-Course/tree/main/Assignment%201/notebooks" target="_blank">notebooks directory</a>.</li>
    <li>Choose any notebook (e.g., <code>MSDS458_Moskowitz_Betzalel_A1_01.ipynb</code>).</li>
    <li>Open it in <a href="https://colab.research.google.com" target="_blank">Google Colab</a>.</li>
    <li>Click <strong>Runtime → Run all</strong> to execute all cells.</li>
  </ol>

  <h2>Files</h2>
  <ul>
    <li><code>notebooks/</code>: Contains multiple Jupyter notebooks testing various architectures</li>
    <li><code>hmtl/</code>: Contains HTML exports of the Jupyter notebooks for offline viewing</li>
    <li><code>Moskowitz_Betzalel_A1.pdf</code>: Final report summarizing experimental design and results</li>
  </ul>

  <h2>Evaluation Metrics</h2>
  <ul>
    <li>Training and test accuracy</li>
    <li>Confusion matrix and classification report</li>
    <li>PCA and t-SNE visualizations of embeddings</li>
  </ul>

  <h2>Citation</h2>
  <blockquote>
    Moskowitz, B. (2023). <em>MNIST Digit Classification with TensorFlow/Keras</em>.
    Assignment 1, MSDS458-DL: Artificial Intelligence and Deep Learning, Northwestern University.
    <a href="https://github.com/betzmosk/Deep-Learning-MSDS-Course/tree/main/Assignment%201" target="_blank">GitHub Repository</a>
  </blockquote>

  <h2>Author</h2>
  <p>
    <strong>Betzalel Moskowitz</strong><br>
    Northwestern University, MSDS Program<br>
    July 2023
  </p>
