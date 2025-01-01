<div align="center">
<h1>
  <br/>项目健康度指标可视化平台
</h1>
</div>

![](https://img.shields.io/badge/License-MIT-blue)
![](https://img.shields.io/badge/Node-v15.14.0-blue)
[![](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-green)](README-CN.md)

![](https://github.com/X-Ethan/2025-1.1-/blob/main/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202025-01-01%20205355.png?raw=true)
![](https://github.com/X-Ethan/2025-1.1-/blob/main/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20250102055304.jpg?raw=true)
![](https://github.com/X-Ethan/2025-1.1-/blob/main/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20250102055351.jpg?raw=true)
![](https://github.com/X-Ethan/2025-1.1-/blob/main/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20250102055206.jpg?raw=true)

The Health Monitor Big Screen is developed as part of the OpenRank competition to evaluate and visualize project health metrics using OpenDigger data.

## About this project

An online-accessible, interactive visualization screen for monitoring and comparing project health metrics. Data is sourced from OpenDigger and processed for visualization and strategic decision-making.

The project is powered by Vue and Echarts, and aims to help enterprises optimize resource allocation and project management strategies.

## How to view ?

### Demo video

[https://www.bilibili.com/video/BV1Nh4y1r7Gt/](https://www.bilibili.com/video/BV1nM6oYKEPR/)

+ Access the application online by typing the following URL into your browser:[项目健康度指标可视化平台](https://github.com/X-Ethan/2025-1.1-/blob/main/index.html)
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

Address: [https://github.com/zxywx0924/openrank](https://github.com/zxywx0924/openrank)

+ Clone the repository locally:

  ```bash
  git clone https://github.com/zxywx0924/openrank.git
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

1. **近期活动次数**: 评估项目是否活跃，吸引新用户或贡献者。在选择开源项目时，开发者希望加入一个活跃度高的项目，因为这通常表明项目被积极维护，问题反馈和功能迭代快速。
2. **新贡献者增长率**: 衡量项目吸引力与社区扩展能力。适用于项目维护团队监控社区的健康状况。当新贡献者增长率较低甚至负增长时，可能表明项目的吸引力下降，需要采取措施（如组织活动、改善文档）。
3. **问题响应率**: 监控社区对用户反馈的支持能力。高响应率能够增强用户和开发者对项目的信心，低响应率则可能导致社区活跃度下降。
4. **代码更改稳定性**:评估项目的稳定性与成熟度。适用于需要长期维护的系统。代码更改不稳定的项目可能会出现频繁的大规模修改，影响版本兼容性。
5. **代码问题密度**:评估项目潜在风险。高代码问题密度可能预示着项目存在代码质量问题，影响开发效率或产品可靠性。
6. **OpenRank趋势**:评估项目在开源生态中的影响力。用于观察项目是否处于快速发展阶段，适用于制定长期合作或投资决策。
7. **变更请求接受率**:评估项目对外部贡献的接受程度。高接受率表明项目对贡献者友好，而低接受率可能使贡献者感到沮丧，从而流失。

#### Data from a wide range of sources

The data for this large screen comes from 

- [X-lab2017](https://github.com/X-lab2017)
- [Github API](https://docs.github.com/en/rest)

The API of X-Lab2017 contains information about a wide variety of open source projects, as follows

![image-20231007232555038](https://markdown-picture-1302861826.cos.ap-shanghai.myqcloud.com/img/2023/10/08/20231008141228.png)

The Github API also allows you to find additional information, such as a map of the project's language distribution.

#### **Dynamic Interactive Queries**

The platform enables interactive querying by project name or author, dynamically updating the visualizations based on user inputs. For example, entering **X-lab2017/open-digger** will display data specific to that repository.
![](https://github.com/X-Ethan/2025-1.1-/blob/main/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20250102055317.jpg?raw=true)

#### **Interactive Charts**

Hover over charts to explore dynamic features like scrolling, zooming, and value highlighting for a more engaging experience.

#### **Comprehensive Insights**

Visualize metrics like 近期活动次数，新贡献者增长率，问题想要率，代码更改稳定性，代码密度问题和OpenRank趋势 to gain a 360-degree view of project health.

### Competition Takeaways

Through this project, the team gained valuable experience in end-to-end data visualization, combining advanced metrics with user-friendly interfaces to promote open-source adoption and enhance decision-making capabilities. Feedback and suggestions are welcome!
