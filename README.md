# qyiai-local-python
#本地化的qyiai
好的，以下是补充后的安装文档：

## 安装步骤

### 1. 安装 Ollama
请根据以下步骤安装 Ollama：

```sh
# 通过以下命令安装 Ollama（请根据您的操作系统选择合适的命令）
# 示例（Linux 或 macOS）：
curl -sSL https://ollama.dev/install.sh | sh

# 示例（Windows，使用 PowerShell）：
iwr -useb https://ollama.dev/install.ps1 | iex
```

### 2. 推送相关模型
安装完成后，您需要将相关的模型推送到 Ollama：

```sh
# 使用以下命令将模型推送到 Ollama
# 比如qwen2
ollama push qwen2 
```

### 3. 模型对应关系在 `config.ini` 中
确保模型对应关系已经在 `config.ini` 文件中正确配置。打开 `config.ini` 文件并检查以下内容：

```ini
[models]
LLM_OLLAMA_MODEL = qwen2
```

### 4. 安装依赖项
使用以下命令安装 `requirements.txt` 文件中的所有依赖项：

```sh
# 使用 pip 安装依赖项
pip install -r requirements.txt
```

### 5. 下载 Ember 模型
请下载 Ember 模型并解压到指定目录：

```sh
# 下载 Ember 模型
wget https://path/to/ember-model.zip

# 解压模型文件
unzip ember-model.zip -d path/to/your/ember-model
```

### 6. 运行 main 测试
一切准备就绪后，运行 `main` 文件进行测试：

```sh
# 运行 main 文件
python main.py
```

### 完成！
按照以上步骤操作后，您应该可以顺利完成安装并运行测试。如有任何问题，请参考相关文档或联系我们的技术支持。

