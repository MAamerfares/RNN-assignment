# 🧠 Simple RNN From Scratch (NumPy Only)

This project demonstrates a basic Recurrent Neural Network (RNN) built **from scratch** using only NumPy. It trains on a toy example to predict the 4th word in a 4-word sequence.

---

## 📋 Task

Given a 3-word input (e.g., `"I love deep"`), the RNN learns to predict the 4th word (`"learning"`).

---

## 🧰 Technologies Used

- Python 3
- NumPy (no deep learning libraries)

---

## 📁 Files

- `rnn_from_scratch.py`: Main Python script containing the full implementation with forward and backward propagation.
- `README.md`: This file.

---

## 🚀 How It Works

1. **Vocabulary Creation**: Converts words to indices and one-hot encodes them.
2. **Forward Pass**:
   - Processes each input word sequentially.
   - Computes hidden states.
   - Outputs a prediction using softmax.
3. **Loss Calculation**: Cross-entropy loss for word prediction.
4. **Backward Pass**:
   - Uses Backpropagation Through Time (BPTT).
   - Calculates gradients for all weights.
5. **Training Loop**:
   - Runs for 100 epochs.
   - Updates weights via gradient descent.

---

## 📈 Sample Output

```
Epoch 0, Loss: 1.3861, Prediction: love
Epoch 10, Loss: 1.3704, Prediction: learning
...
Epoch 90, Loss: 1.2045, Prediction: learning
```

---

## 🏁 To Run

Make sure you have Python and NumPy installed. Then run:

```bash
python rnn_from_scratch.py
```

---

## 💡 Notes

- This is a **minimal educational implementation**—ideal for understanding how RNNs work internally.
- Gradients are clipped to avoid exploding gradients.

---

## 📚 License

MIT License

