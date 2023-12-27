we use the short-term trading multi-factor alpha stock selection system, known as the 191 Alphas, which only operates on four basic dimensions: opening price, closing price, highest price, lowest price, and trading volume. The factors measure abnormal detection of opening price, abnormal detection of periodic trading volume, abnormal fluctuations in price on the same day, and other aspects.
We design a CNN-LSTM model based on the Attention mechanism, which can effectively capture local and global dependencies in sequential data.
Attention can improve the effect of important time steps in LSTM, thereby further reducing the model prediction error. Attention essentially involves calculating the weighted average of the output vectors of the last layer of LSTM. The output vectors of the hidden layers of LSTM are used as inputs to the attention layer, which is trained through a fully connected layer. The weight size represents the importance of the hidden state at each time step for the prediction result.
After repeated testing, we adopted ELU as the activation function in the convolutional layer and LSTM layer, and tanh as the activation function in the final fully connected layer.
