# mnist-simple-nn
极简神经网络：手写数字识别 (MNIST)
这是一个基于 PyTorch 的深度学习入门项目，使用了最基础的两层 MLP (784 -> 128 -> 10) 实现 MNIST 手写数字识别。

## ✨ 项目亮点
- **底层原理实现**：不依赖 `nn.Module`，纯用 `torch.tensor` 和 autograd 手动实现前向传播、反向传播和参数更新（手写版）。
- **工程化实现**：用 `nn.Module` 和 `torch.optim` 重构，代码更简洁。
- **交互式画板**：基于 `ipycanvas` 实现了一个浏览器内的手写画板，可以实时测试模型效果。
- **可视化**：包含训练 Loss / 测试准确率曲线，以及预测结果的可视化。



## 🛠️ 环境安装

本项目在 Python 3.9+ 和 PyTorch 2.8.0 (CUDA 12.6) 下测试通过。

### 安装依赖
如果你需要完全相同的 GPU 环境，请运行以下命令：
```bash
pip install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cu126

注：如果你没有 NVIDIA GPU 或者 CUDA 版本不同，请修改 requirements.txt，将带有 +cu126 的行改为 torch 和 torchvision（不指定版本），或者前往 PyTorch 官网 获取适合你电脑的安装命令。
