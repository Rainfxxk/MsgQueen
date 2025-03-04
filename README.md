# MsgQueen：基于消息队列的网络框架

## 项目简介

MsgQueen是一个轻量级且高效的网络框架，旨在通过消息队列实现分布式系统之间的通信。

## 主要特性
- **异步通信**：实现组件之间的无缝交互，无需阻塞。
- **解耦**：分离应用程序不同部分的职责，便于维护和扩展。
- **可扩展性**：根据需要轻松添加更多生产者或消费者以扩展应用程序。
- **跨平台支持**：兼容多种操作系统和编程环境。

## 快速开始

### 前置条件
- **Python 3.8+**：MsgQueen 使用 Python 构建，因此请确保已安装 Python 3.8 或更高版本。

### 配置
在 `netconfig.py` 文件中配置你的消息队列服务设置。示例：
```python
# netconfig.py
host = "127.0.0.1"

port = "2004"

package_size = 848

package_header_size = 12

package_data_size = package_size - package_header_size

charset = "utf-8"
```

### 运行示例
运行示例生产者和消费者脚本，查看 MsgQueen 的实际运行效果：
```bash
python main_recv.py
python main_send.py
```