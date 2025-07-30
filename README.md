# LSTM - Text Classification
The project presents the implementation of an LSTM network for Polish text classification using the BAN‑PL corpus. Four experiments were conducted to analyze how the classifier’s performance is affected by: text preprocessing, word embedding layers, LSTM network architecture, and hyperparameter optimization.

# Results
## 1. Text preprocessing
<table>
  <thead>
    <tr>
      <th width="200px" align="center">Text preprocessing</th>
      <th align="center">Accuracy</th>
      <th align="center">Precision</th>
      <th align="center">Recall</th>
      <th align="center">F1‑score</th>
      <th align="center">Training time</th>
      <th align="center">Epoch</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Basic</strong></td>
      <td align="center">81.41%</td>
      <td align="center">80.06%</td>
      <td align="center">83.66%</td>
      <td align="center">81.82%</td>
      <td align="center">0:02:25</td>
      <td align="center">6</td>
    </tr>
    <tr>
      <td align="center"><strong>Lemmatization</strong></td>
      <td align="center">84.08%</td>
      <td align="center">84.25%</td>
      <td align="center">83.83%</td>
      <td align="center">84.04%</td>
      <td align="center">0:01:28</td>
      <td align="center">6</td>
    </tr>
    <tr>
      <td align="center"><strong>Lemmatization + Stop‑words Removal</strong></td>
      <td align="center">84.62%</td>
      <td align="center">83.26%</td>
      <td align="center">86.66%</td>
      <td align="center">84.93%</td>
      <td align="center">0:02:25</td>
      <td align="center">6</td>
    </tr>
  </tbody>
</table>

## 2. Word embedding layers
<table>
  <thead>
    <tr>
      <th width="200px" align="center">Embedding</th>
      <th align="center">Accuracy</th>
      <th align="center">Precision</th>
      <th align="center">Recall</th>
      <th align="center">F1‑score</th>
      <th align="center">Training time</th>
      <th align="center">Epoch</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>Basic</strong></td>
      <td align="center">84.62%</td>
      <td align="center">83.26%</td>
      <td align="center">86.66%</td>
      <td align="center">84.93%</td>
      <td align="center">0:02:25</td>
      <td align="center">6</td>
    </tr>
    <tr>
      <td align="center"><strong>Pre‑trained Word2Vec</strong></td>
      <td align="center">85.95%</td>
      <td align="center">85.69%</td>
      <td align="center">86.33%</td>
      <td align="center">86.01%</td>
      <td align="center">0:01:52</td>
      <td align="center">7</td>
    </tr>
    <tr>
      <td align="center"><strong>Pre‑trained FastText</strong></td>
      <td align="center">85.87%</td>
      <td align="center">85.43%</td>
      <td align="center">86.50%</td>
      <td align="center">85.96%</td>
      <td align="center">0:17:26</td>
      <td align="center">6</td>
    </tr>
  </tbody>
</table>

## 3. LSTM network architecture
<table>
  <thead>
    <tr>
      <th width="200px" align="center">Model</th>
      <th align="center">Accuracy</th>
      <th align="center">Precision</th>
      <th align="center">Recall</th>
      <th align="center">F1‑score</th>
      <th align="center">Training time</th>
      <th align="center">Epoch</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>LSTM</strong></td>
      <td align="center">85.95%</td>
      <td align="center">85.69%</td>
      <td align="center">86.33%</td>
      <td align="center">86.01%</td>
      <td align="center">0:01:52</td>
      <td align="center">7</td>
    </tr>
    <tr>
      <td align="center"><strong>BiLSTM</strong></td>
      <td align="center">86.33%</td>
      <td align="center">87.91%</td>
      <td align="center">84.25%</td>
      <td align="center">86.04%</td>
      <td align="center">0:02:11</td>
      <td align="center">6</td>
    </tr>
    <tr>
      <td align="center"><strong>BERT</strong></td>
      <td align="center">88.29%</td>
      <td align="center">86.32%</td>
      <td align="center">91.00%</td>
      <td align="center">88.60%</td>
      <td align="center">1:13:02</td>
      <td align="center">8</td>
    </tr>
  </tbody>
</table>

## 4. Hyperparameter optimization
<table>
  <thead>
    <tr>
      <th align="center">Accuracy</th>
      <th align="center">Precision</th>
      <th align="center">Recall</th>
      <th align="center">F1‑score</th>
      <th align="center">Optimization time</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">87.95%</td>
      <td align="center">86.76%</td>
      <td align="center">89.58%</td>
      <td align="center">88.15%</td>
      <td align="center">0:40:03</td>
    </tr>
  </tbody>
</table>
