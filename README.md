# 狂飙演员爬虫与数据分析 

本项目基于 Scrapy 框架，自动爬取百度百科中《狂飙》电视剧的演员信息，并使用 matplotlib 对演员的星座、身高、体重进行可视化分析。

---

## 🚀 功能亮点

- ✅ 自动爬取演员姓名与百科链接
- ✅ 提取演员的出生日期、星座、身高、体重等属性
- ✅ 输出为 JSON 文件，便于后续分析
- ✅ 使用 matplotlib 绘制星座柱状图、身高饼图、体重分布图
- ✅ 提供交互式菜单，一键查看分析结果

---


## 🛠️ 使用方法

### 1️⃣ 安装依赖

```bash
conda create -n kb_spider python=3.10
conda activate kb_spider
pip install scrapy matplotlib
```

### 2️⃣ 运行爬虫
```bash
# 抓取演员链接
scrapy crawl KB

# 抓取演员详细信息
scrapy crawl actor_Info
输出结果将保存在 actors_link.json 和 actors_info.json
```
### 3️⃣ 分析数据
```bash
python analyse.py
```
控制台将显示交互菜单，选择对应项即可查看图表
