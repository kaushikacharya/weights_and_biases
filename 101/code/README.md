# Assignments

## Intro to W&B

- Description
  - Run an experiment by passing hyperparameters.
  - Log metrics.
  - Visualize results in dashboard.

- **Notebooks**
  - [Google Colab](https://colab.research.google.com/drive/1GqU8SKVFiZwFWAIqepG_FDjXpS7r9ZqS)
  - [Local](./Intro_to_Weights_&_Biases.ipynb)

## Simple PyTorch Integration

- Description
  - Train MNIST classifier using a [Convolutional Neural Network](https://github.com/kaushikacharya/Introduction_to_Deep_Learning_and_Neural_Networks/blob/master/notes/Chapter_3.md#convolutional-neural-networks).
  - Track gradients using ```wandb.watch```.
  - Save the model in onnx format.

- **Notebook**
  - [Local](./Simple_PyTorch_Integration.ipynb)

- **Computation**
  - Image tensor size output of CNN steps are explained in the documentation of [Conv2d](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html) and [MaxPool2d](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html).

- **Learnings**
  - Flatten CNN output tensor
    - Here we have used the command ```x.reshape(x.size(0), -1)```.
    - Alternatively, as shown in [Deep Learning and Neural Networks course](https://github.com/kaushikacharya/Introduction_to_Deep_Learning_and_Neural_Networks/blob/master/notes/Chapter_3.md#build-a-convolutional-network) we can use ```x.view(-1, x.shape[-3]*x.shape[-2]*x.shape[-1])```
  - [torch.onnx.export](https://pytorch.org/docs/stable/onnx.html#tracing-vs-scripting)
  - libcuda.so not found in WSL2:
    - ```Could not load library libcudnn_cnn_infer.so.8. Error: libcuda.so: cannot open shared object file: No such file or directory```
    - **Environment**: Ubuntu 22.04.2 LTS (GNU/Linux 5.15.90.1-microsoft-standard-WSL2 x86_64)
    - Workaround solution for this [issue in WSL](https://github.com/m4rs-mt/ILGPU/issues/1008#issuecomment-1579651512) is mentioned in [WSL repository's discussion thread](https://github.com/microsoft/WSL/issues/8587#issuecomment-1229170859).
  