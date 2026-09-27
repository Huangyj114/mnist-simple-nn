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
```
注：如果你没有 NVIDIA GPU 或者 CUDA 版本不同，请修改 requirements.txt，将带有 +cu126 的行改为 torch 和 torchvision（不指定版本），或者前往 PyTorch 官网 获取适合你电脑的安装命令。

📊 结果展示
<img width="1417" height="457" alt="7c844bae6f7839494b133425f483cb8" src="https://github.com/user-attachments/assets/54ab1488-ddf0-40ca-b10f-c967b2377121" />

<img width="816" height="879" alt="aec58271c531ad2c7b0fccb716f8071" src="https://github.com/user-attachments/assets/17d76b00-038b-48cf-8af2-28f5a402baaf" />

<img width="781" height="884" alt="b8cc66a792f05c64867cf484eb94ba5" src="https://github.com/user-attachments/assets/8f256c6a-0ec4-4d5e-95c4-560277488b9e" />

<img width="766" height="891" alt="56847fa2f9b637ab9d1e37037a34084" src="https://github.com/user-attachments/assets/a1d6bbe9-70bf-49fe-9a2d-5ce3669111d9" />

<img width="784" height="880" alt="bfaf94b86098f2aeda58b548fcecffd" src="https://github.com/user-attachments/assets/d8689052-bc5d-48fb-880c-e2d76e042b14" />




本项目地址：github.com/Huangyj114/mnist-simple-nn
