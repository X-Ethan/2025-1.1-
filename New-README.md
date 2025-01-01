<div align="center">
<h1>
  <br/>项目健康度指标可视化平台
</h1>
</div>

![](https://img.shields.io/badge/License-MIT-blue)
![](https://img.shields.io/badge/Node-v15.14.0-blue)
[![](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-green)](README-CN.md)

![示例图片](https://github.com/X-Ethan/2025-1.1-/blob/main/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-01-01%20205355.png?raw=true)

The Health Monitor Big Screen is developed as part of the OpenRank competition to evaluate and visualize project health metrics using OpenDigger data.

## About this project

An online-accessible, interactive visualization screen for monitoring and comparing project health metrics. Data is sourced from OpenDigger and processed for visualization and strategic decision-making.

The project is powered 🚀 by Vue and Echarts, and aims to help enterprises optimize resource allocation and project management strategies.

## How to view ?

### Demo video

[https://www.bilibili.com/video/BV1Nh4y1r7Gt/](https://www.bilibili.com/video/BV1nM6oYKEPR/)

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
