<h1>Assignment 3: A Comparative Study of Neural Network Architectures for Intent Recognition</h1>

  <h2>Overview</h2>
  <p>
    This project explores various deep learning architectures for the task of text classification using the AG News dataset. 
    It serves as a proxy problem for intent recognition in conversational agents. The main goal was to assess the effectiveness 
    of different neural network topologies, representation methods, and vocabulary sizes on classification performance.
  </p>

  <h2>Key Architectures Evaluated</h2>
  <ul>
    <li><strong>Fully Connected Dense Networks (DNNs)</strong> - 4-layer models with tanh activation</li>
    <li><strong>Recurrent Neural Networks (RNNs)</strong> - Unidirectional and Bidirectional</li>
    <li><strong>Long Short-Term Memory Networks (LSTMs)</strong> - Unidirectional and Bidirectional</li>
    <li><strong>Gated Recurrent Units (GRUs)</strong> - Multiple variants with and without dropout</li>
    <li><strong>1D Convolutional Neural Networks (CNNs)</strong> - Both single-layer and two-layer models with dropout</li>
  </ul>

  <h2>Experimental Variables</h2>
  <ul>
    <li><strong>Representation Methods:</strong> One-hot encoding vs. dense embeddings</li>
    <li><strong>Vocabulary Sizes:</strong> 1,000 vs. 10,000 tokens</li>
    <li><strong>Sequence Length:</strong> Fixed at 40 tokens per input</li>
    <li><strong>Regularization:</strong> Dropout, recurrent dropout, and early stopping</li>
  </ul>

  <h2>Technologies Used</h2>
  <ul>
    <li><strong>Platform:</strong> Google Colab (with T4 GPU)</li>
    <li><strong>Framework:</strong> Keras with TensorFlow 2.12</li>
    <li><strong>Visualization:</strong> Matplotlib, Seaborn</li>
    <li><strong>Libraries:</strong> Pandas, NumPy</li>
  </ul>

  <h2>How to Run</h2>
  <ol>
    <li>Open any of the notebook HTML exports (e.g., <code>MSDS458_Moskowitz_Betzalel_GRU.html</code>) in a browser to review the code and results.</li>
    <li>If you want to re-run or adapt the experiments, replicate the architectures described in the paper within a Google Colab notebook using TensorFlow/Keras.</li>
    <li>Ensure that you load and preprocess the AG News dataset as described, and set up early stopping and dropout as needed.</li>
  </ol>

  <h2>Best Performing Model</h2>
  <p>
    The top-performing model was a GRU using dense embeddings with a vocabulary size of 10,000 and 20% dropout. 
    It achieved a test accuracy of <strong>90.75%</strong>.
  </p>

  <h2>Findings</h2>
  <ul>
    <li>GRUs and LSTMs with dense embeddings consistently outperformed other architectures.</li>
    <li>Increasing vocabulary size had a significant positive effect on performance.</li>
    <li>Embedding representations yielded higher accuracy but were more prone to overfitting.</li>
    <li>Fully connected dense models performed poorly on their own, underscoring the importance of sequential architectures for NLP tasks.</li>
  </ul>

  <h2>Future Work</h2>
  <p>
    Future directions include fine-tuning transformer-based models like BERT or XLNet, experimenting with larger vocabulary sizes, 
    and employing advanced regularization techniques or dimensionality reduction methods like t-SNE for further analysis.
  </p>

  <h2>Citation</h2>
  <p>If you use this work in your own research or projects, please cite:</p>
  <pre>
Moskowitz, B. (2023). A Comparative Study of Neural Network Architectures for Intent Recognition.
MSDS458 - Deep Learning, Northwestern University.
Available at: https://github.com/betzmosk/Deep-Learning-MSDS-Course/tree/main/Assignment%203
  </pre>

  <h2>Author</h2>
  <p><strong>Betzalel Moskowitz</strong><br>
  MSDS458 - Artificial Intelligence and Deep Learning<br>
  August 2023</p>
