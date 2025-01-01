<div align="center">
<h1>
  <br/>项目健康度指标可视化平台
</h1>
</div>

![](https://img.shields.io/badge/License-MIT-blue)
![](https://img.shields.io/badge/Node-v15.14.0-blue)
[![](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-green)](README-CN.md)

![](https://markdown-picture-1302861826.cos.ap-shanghai.myqcloud.com/img/2025/01/01/health-visualization-platform.png)

The Health Monitor Big Screen is developed as part of the OpenRank competition to evaluate and visualize project health metrics using OpenDigger data.

## About this project

An online-accessible, interactive visualization screen for monitoring and comparing project health metrics. Data is sourced from OpenDigger and processed for visualization and strategic decision-making.

The project is powered 🚀 by Vue and Echarts, and aims to help enterprises optimize resource allocation and project management strategies.

## How to view ?

### Demo video

[Click here to watch the demo video](https://www.bilibili.com/video/BV1Nh4y1r7Gt/)

+ Access the application online by typing the following URL into your browser: [http://open-health-monitor.com/#/](http://open-health-monitor.com/#/)

### Docker deployment

1. **Install Docker**: Ensure Docker is installed on your system. Follow the instructions in the official documentation: [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/).

2. **Pull images**: Download the Docker image for the application using the following command:

   ```bash
   docker pull openrank/health-monitor:latest
   ```

3. **Run the container**: Start the application by running:

   ```bash
   docker run -d -p 8081:8081 openrank/health-monitor
   ```

   - The `-d` flag runs the container in the background.
   - The `-p 8081:8081` maps the container's port to the host system.

4. **Access the application**: Once the container is running, open `http://localhost:8081` in your browser to access the application. Use `docker stop container-id` to stop the container when needed.

### Github repository clone

Address: [https://github.com/YourRepository/HealthMonitorBigScreen](https://github.com/YourRepository/HealthMonitorBigScreen)

+ Clone the repository locally:

  ```bash
  git clone https://github.com/YourRepository/HealthMonitorBigScreen.git
  ```

+ Install dependencies (Node.js version 15.14.0 is recommended):

  ```bash
  cd HealthMonitorBigScreen
  npm install
  ```

+ Run the application (default port: 8080):

  ```bash
  npm run serve
  ```

## Introduction to the Health Monitor Visualization Screen

### Scenario and meaning

Monitoring project health is crucial for enterprises to identify high-potential projects, optimize resource allocation, and mitigate risks. By visualizing health metrics such as activity, community engagement, code quality, and development trends, the application helps stakeholders make informed decisions efficiently.

### Realization

The data for this big screen is sourced from:

- [OpenDigger](https://github.com/X-lab2017/open-digger)
- [Github API](https://docs.github.com/en/rest)

Technology stack: Vue 2.6, Echarts 5.3, RESTful API.

### Description of the work

#### **Thumbnail of the big screen**

![](https://markdown-picture-1302861826.cos.ap-shanghai.myqcloud.com/img/2023/10/16/20231016021040.gif)

### Key Features

#### **Health Metrics**

1. **Activity Metrics**: Monitor recent activity frequency and new contributor growth rate to evaluate project vibrancy and attractiveness.
2. **Community Engagement Metrics**: Assess participant diversity and issue response rates to gauge global reach and feedback support capabilities.
3. **Code Quality Metrics**: Analyze code change stability and issue density to evaluate project maturity and stability.
4. **Development Metrics**: Observe OpenRank trends and pull request acceptance rates to understand project influence and contributor-friendliness.

#### **Dynamic Interactive Queries**

The platform enables interactive querying by project name or author, dynamically updating the visualizations based on user inputs. For example, entering **angular/angular** will display data specific to that repository.

#### **Interactive Charts**

Hover over charts to explore dynamic features like scrolling, zooming, and value highlighting for a more engaging experience.

#### **Comprehensive Insights**

Visualize metrics like language composition, contributor word clouds, project star trends, and OpenRank trends to gain a 360-degree view of project health.

### Competition Takeaways

Through this project, the team gained valuable experience in end-to-end data visualization, combining advanced metrics with user-friendly interfaces to promote open-source adoption and enhance decision-making capabilities. Feedback and suggestions are welcome!
<div align="center">
<h1>
  <br/>项目健康度指标可视化平台
</h1>
</div>

![](https://img.shields.io/badge/License-MIT-blue)
![](https://img.shields.io/badge/Node-v15.14.0-blue)
[![](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-green)](README-CN.md)

![](/mnt/data/屏幕截图%202025-01-01%20164246.png)

## 关于此项目

此项目是 OpenRank 比赛的一部分，旨在利用 OpenDigger 数据评估和可视化项目健康指标。

一个在线可访问的交互式可视化大屏，用于监控和比较项目健康指标。数据来源于 OpenDigger，并经过处理以实现可视化和战略决策。

项目基于 Vue 和 Echarts 构建，帮助企业优化资源分配和项目管理策略。

## 如何查看？

### 演示视频

[点击此处观看演示视频](https://www.bilibili.com/video/BV1Nh4y1r7Gt/)

+ 在浏览器中输入以下 URL 访问应用程序：[http://open-health-monitor.com/#/](http://open-health-monitor.com/#/)

### Docker 部署

1. **安装 Docker**: 确保系统已安装 Docker。请参考官方文档：[https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)。

2. **拉取镜像**: 使用以下命令下载应用程序的 Docker 镜像：

   ```bash
   docker pull openrank/health-monitor:latest
   ```

3. **运行容器**: 使用以下命令启动应用程序：

   ```bash
   docker run -d -p 8081:8081 openrank/health-monitor
   ```

   - `-d` 标志表示容器将在后台运行。
   - `-p 8081:8081` 将容器的端口映射到主机系统。

4. **访问应用程序**: 容器运行后，在浏览器中打开 `http://localhost:8081` 即可访问应用程序。需要停止容器时可使用 `docker stop container-id`。

### 克隆 Github 仓库

地址：[https://github.com/YourRepository/HealthMonitorBigScreen](https://github.com/YourRepository/HealthMonitorBigScreen)

+ 本地克隆仓库：

  ```bash
  git clone https://github.com/YourRepository/HealthMonitorBigScreen.git
  ```

+ 安装依赖项（推荐 Node.js 版本为 15.14.0）：

  ```bash
  cd HealthMonitorBigScreen
  npm install
  ```

+ 运行应用程序（默认端口：8080）：

  ```bash
  npm run serve
  ```
