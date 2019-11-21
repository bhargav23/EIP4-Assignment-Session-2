# EIP4-Assignment-Session-2
## Log
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 16s 262us/step - loss: 0.2330 - acc: 0.9261 - val_loss: 0.0568 - val_acc: 0.9814
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 11s 177us/step - loss: 0.0740 - acc: 0.9766 - val_loss: 0.0405 - val_acc: 0.9854
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0564 - acc: 0.9821 - val_loss: 0.0432 - val_acc: 0.9863
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0477 - acc: 0.9842 - val_loss: 0.0305 - val_acc: 0.9896
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 11s 176us/step - loss: 0.0447 - acc: 0.9861 - val_loss: 0.0265 - val_acc: 0.9909
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0418 - acc: 0.9867 - val_loss: 0.0240 - val_acc: 0.9916
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0371 - acc: 0.9882 - val_loss: 0.0204 - val_acc: 0.9935
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 10s 173us/step - loss: 0.0342 - acc: 0.9890 - val_loss: 0.0243 - val_acc: 0.9922
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 11s 175us/step - loss: 0.0332 - acc: 0.9892 - val_loss: 0.0220 - val_acc: 0.9928
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 10s 175us/step - loss: 0.0305 - acc: 0.9904 - val_loss: 0.0198 - val_acc: 0.9933
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0286 - acc: 0.9907 - val_loss: 0.0227 - val_acc: 0.9928
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 10s 175us/step - loss: 0.0307 - acc: 0.9905 - val_loss: 0.0233 - val_acc: 0.9926
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 10s 175us/step - loss: 0.0279 - acc: 0.9907 - val_loss: 0.0229 - val_acc: 0.9934
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0265 - acc: 0.9912 - val_loss: 0.0193 - val_acc: 0.9944
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 11s 176us/step - loss: 0.0261 - acc: 0.9916 - val_loss: 0.0202 - val_acc: 0.9938
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 10s 174us/step - loss: 0.0252 - acc: 0.9919 - val_loss: 0.0220 - val_acc: 0.9938
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 11s 178us/step - loss: 0.0256 - acc: 0.9919 - val_loss: 0.0188 - val_acc: 0.9935
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 11s 175us/step - loss: 0.0238 - acc: 0.9920 - val_loss: 0.0189 - val_acc: 0.9943
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 11s 176us/step - loss: 0.0230 - acc: 0.9926 - val_loss: 0.0166 - val_acc: 0.9955
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 10s 175us/step - loss: 0.0234 - acc: 0.9924 - val_loss: 0.0160 - val_acc: 0.9941
<keras.callbacks.History at 0x7f7c72971438>

## model.evaluate (on test data)
[0.016032473114388993, 0.9941]

## Strategy

* To reduce the number of parameters, I updated the second layer of convolution from 32 to 16. Then the number of parameters reduced to less than 15000, I, e. 14020.
* To improve the accuracy, I added the Batch normalization and drop out after every convolution layer but not in the last layer.
* The drop out rate is set to 15%.



