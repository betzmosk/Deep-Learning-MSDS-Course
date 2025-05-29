<h1>Assignment 2: Suitability of Deep Learning Architectures for Facial Recognition</h1>

  <p><strong>Author:</strong> Betzalel Moskowitz<br>
  <strong>Course:</strong> MSDS458-DL: Artificial Intelligence and Deep Learning<br>
  <strong>Date:</strong> July 23, 2023</p>

  <h2>Overview</h2>
  <p>This project explores the effectiveness of various deep learning architectures for image classification tasks as a proxy for facial recognition systems. Experiments were conducted using the CIFAR-10 dataset to compare performance across different network types and regularization techniques. The results provide insights into why convolutional neural networks (CNNs) dominate modern facial recognition solutions.</p>

  <h2>Objectives</h2>
  <ul>
    <li>Evaluate fully connected deep neural networks (DNNs) vs. convolutional neural networks (CNNs).</li>
    <li>Analyze the effects of hyperparameters (batch size, number of nodes, etc.).</li>
    <li>Investigate the impact of regularization methods (dropout, batch normalization, L2 regularization).</li>
  </ul>

  <h2>Dataset</h2>
  <p>The experiments use the CIFAR-10 dataset, which contains 60,000 labeled color images (32x32 pixels), spread across 10 classes. It serves as a practical stand-in for more complex facial recognition datasets.</p>

  <h2>Key Findings</h2>
  <ul>
    <li>Simple DNNs achieved <strong>~50% accuracy</strong>.</li>
    <li>CNNs with proper regularization exceeded <strong>82% test accuracy</strong>.</li>
    <li>Regularization (especially L2 + batch norm + dropout) significantly reduces overfitting.</li>
    <li>The best-performing model was a 6-layer CNN (Model 5b) with a test accuracy of <strong>82.68%</strong>.</li>
  </ul>

  <h2>Code Execution</h2>
  <p>The original code was run in Google Colab and is not included in the repo. However, HTML exports of the code output can be viewed in the <code><a href="https://github.com/betzmosk/Deep-Learning-MSDS-Course/tree/main/Assignment%202/html">Assignment 2</a></code> directory.</p>

  <h2>Dependencies</h2>
  <ul>
    <li><code>tensorflow==2.12</code></li>
    <li><code>keras</code></li>
    <li><code>numpy</code></li>
    <li><code>pandas</code></li>
    <li><code>matplotlib</code></li>
    <li><code>seaborn</code></li>
    <li><code>sklearn</code></li>
  </ul>

  <h2>Paper</h2>
  <p>You can read the full project report here: 
    <a href="https://github.com/betzmosk/Deep-Learning-MSDS-Course/blob/main/Assignment%202/Moskowitz_Betzalel_A2.pdf" target="_blank">Moskowitz_Betzalel_A2.pdf</a>
  </p>

  <h2>Citation</h2>
  <p>If you wish to cite this work, please use:</p>
  <pre>
Moskowitz, B. (2023). Suitability of Deep Learning Architectures for Facial Recognition. MSDS458-DL Final Assignment. https://github.com/betzmosk/Deep-Learning-MSDS-Course/tree/main/Assignment%202
  </pre>

  <h2>License</h2>
  <p>© 2023 Betzalel Moskowitz. All rights reserved. For academic use only.</p>
