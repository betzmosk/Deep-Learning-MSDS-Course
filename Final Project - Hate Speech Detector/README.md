<h1>Hate Speech Detection Using Deep Learning</h1>

  <p>
    This project was developed as the final assignment for the MSDS458-DL: Artificial Intelligence and Deep Learning course at Northwestern University.
    It explores the use of various deep learning architectures for binary hate speech detection on social media text.
  </p>

  <h2>Overview</h2>
  <p>
    Hate speech presents a major challenge for online communities and platforms.
    This project aims to build robust automated hate speech detection models capable of distinguishing hateful from non-hateful content.
    The study evaluates traditional bag-of-words approaches alongside modern sequence models, CNN/RNN hybrids, and transformer-based architectures.
  </p>

  <h2>Key Findings</h2>
  <ul>
    <li>Bag-of-bigrams models using TF-IDF significantly outperformed most deep learning sequence models.</li>
    <li>The best-performing model achieved <strong>86.2% test accuracy</strong> and <strong>86% precision, recall, and F1 scores</strong>.</li>
    <li>Fine-tuned GloVe embeddings within CNN-LSTM hybrids showed strong performance.</li>
    <li>Transformer models underperformed unless combined with pretrained embeddings.</li>
  </ul>

  <h2>Dataset</h2>
  <ul>
    <li><strong>Source:</strong> Mody et al. (2023)</li>
    <li><strong>Labels:</strong> 1 = Hate Speech, 0 = Non-Hateful</li>
    <li><strong>Preprocessing:</strong> Emoji-to-text, link and mention removal, contraction expansion, punctuation stripping, vocabulary cap of 50,000 words.</li>
    <li>Stratified-sampled subset: ~363,000 samples (train/val/test).</li>
  </ul>

  <h2>Models Implemented</h2>
  <h3>Bag-of-Words Models (TF-IDF Bigrams)</h3>
  <ul>
    <li>DNNs with dropout and batch normalization.</li>
  </ul>

  <h3>Sequence Models</h3>
  <ul>
    <li>BiLSTM and BiGRU with embedding layers.</li>
    <li>1D CNNs with global pooling.</li>
    <li>Hybrid CNN + RNN models inspired by Zhang et al. (2018).</li>
    <li>Transformer encoders with positional or GloVe embeddings.</li>
  </ul>

  <h3>Transfer Learning</h3>
  <ul>
    <li>GloVe embeddings (frozen and fine-tuned).</li>
  </ul>

  <h2>Technologies Used</h2>
  <ul>
    <li>Google Colab with A100 GPU</li>
    <li>TensorFlow / Keras</li>
    <li>NumPy, pandas, scikit-learn</li>
    <li>Matplotlib, Seaborn</li>
  </ul>

  <h2>Performance Summary</h2>
  <table border="1" cellspacing="0" cellpadding="4">
    <thead>
      <tr>
        <th>Model Type</th>
        <th>Test Accuracy</th>
        <th>Test F1</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>TF-IDF Bigrams + DNN</td><td><strong>86.2%</strong></td><td><strong>86%</strong></td></tr>
      <tr><td>CNN + LSTM + GloVe (Fine-tuned)</td><td>85.5%</td><td>85%</td></tr>
      <tr><td>Transformer + GloVe (Fine-tuned)</td><td>85.1%</td><td>85%</td></tr>
      <tr><td>BiGRU</td><td>84.4%</td><td>84%</td></tr>
      <tr><td>Transformer (4 heads)</td><td>84.4%</td><td>84%</td></tr>
      <tr><td>CNN (128 filters)</td><td>83.3%</td><td>83%</td></tr>
    </tbody>
  </table>

  <h2>How to Run</h2>
  <ol>
    <li>Open <code>notebook.ipynb</code> in Google Colab or locally.</li>
    <li>Run all cells to train and evaluate models.</li>
    <li>Modify architecture blocks to explore further experiments.</li>
  </ol>

  <h2>Paper</h2>
  <p>
    See <code>Moskowitz_Betzalel_FinalProject.pdf</code> for the full research paper including:
    <ul>
      <li>Background, dataset details, and ethical considerations</li>
      <li>Model design rationale</li>
      <li>Experiment methodology and results</li>
      <li>References</li>
    </ul>
  </p>

  <h2>Citation</h2>
  <p>If you use or reference this work in your research, please cite:</p>
  <blockquote>
    Moskowitz, B. (2023). <i>Deep Learning for Hate Speech Detection</i>. Final Project, MSDS458-DL: Artificial Intelligence and Deep Learning, Northwestern University. <a href="https://github.com/betzmosk/Deep-Learning-MSDS-Course/tree/main/Final%20Project%20-%20Hate%20Speech%20Detector">GitHub Repository</a>
  </blockquote>

  <h2>Author</h2>
  <p>
    <strong>Betzalel Moskowitz</strong><br>
    Northwestern University, MSDS Program<br>
    August 2023
  </p>
