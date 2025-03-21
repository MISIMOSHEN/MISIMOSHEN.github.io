<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mimoshen | 运动生态学研究</title>
    <style>
        :root {
            --primary: #2D5D4B;  /* 森林绿 */
            --secondary: #6B8F71; /* 苔藓绿 */
            --accent: #A4C3B2;    /* 雾霾绿 */
            --text: #36453B;      /* 深灰绿 */
            --background: #F8F9FA;
        }

        body {
            font-family: 'Segoe UI', system-ui;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            background: var(--background);
            color: var(--text);
        }

        .section {
            max-width: 800px;
            margin: 40px auto;
            padding: 25px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .experience-card {
            border-left: 4px solid var(--primary);
            padding-left: 20px;
            margin: 25px 0;
            transition: transform 0.3s;
        }

        .experience-card:hover {
            transform: translateX(10px);
        }

        .skill-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .skill-card {
            background: var(--accent);
            padding: 12px;
            border-radius: 8px;
            text-align: center;
        }

        h2 {
            color: var(--primary);
            border-bottom: 2px solid var(--secondary);
            padding-bottom: 5px;
        }

        .timeline {
            color: #666;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <div class="section">
        <h1>🐾 Mimoshen</h1>
        <p>👋 运动生态学研究者 | 野生动物保护技术专家</p>
    </div>

    <div class="section">
        <h2>🔍 研究经历</h2>
        
        <div class="experience-card">
            <h3>野外研究助理 · 龙口林场</h3>
            <div class="timeline">2022.11 - 哈尔滨</div>
            <ul>
                <li>应用隐马尔可夫模型验证野猪运动模式</li>
                <li>开发行为识别算法，提升研究准确度15%</li>
            </ul>
        </div>

        <div class="experience-card">
            <h3>野生动物救援志愿者 · 珲春市</h3>
            <ul>
                <li>参与野猪项圈安装与放归的完整流程</li>
                <li>操作VHF/GPS混合追踪系统</li>
                <li>收集超过200小时的野生动物活动数据</li>
            </ul>
        </div>

        <div class="experience-card">
            <h3>太平沟自然保护区 · 2023</h3>
            <ul>
                <li>使用无人机技术进行梅花鹿种群调查</li>
                <li>设计10公里样线调查方案</li>
                <li>建立物种分布预测模型（精度92%）</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2>🛠️ 技术能力</h2>
        <div class="skill-grid">
            <div class="skill-card">Home Range Analysis</div>
            <div class="skill-card">轨迹可视化</div>
            <div class="skill-card">UD建模</div>
            <div class="skill-card">数据清洗</div>
            <div class="skill-card">行为模式识别</div>
            <div class="skill-card">活动范围重叠分析</div>
        </div>
    </div>

    <div class="section">
        <h2>📬 联系合作</h2>
        <p>寻求以下合作：</p>
        <ul>
            <li>野生动物追踪技术优化</li>
            <li>保护地管理数据分析</li>
            <li>动物行为模型开发</li>
        </ul>
        <p>📧 联系方式: [你的邮箱]</p>
    </div>
</body>
</html>
<div id="research-map" style="height: 400px;"></div>
<script>
    const map = L.map('research-map').setView([45.8, 126.5], 6);
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png').addTo(map);
    
    // 添加研究地点标记
    const markers = [
        {loc: [44.04, 129.08], title: '珲春野猪研究'},
        {loc: [45.32, 130.9], title: '太平沟梅花鹿'}
    ];
    
    markers.forEach(m => {
        L.marker(m.loc)
         .bindPopup(m.title)
         .addTo(map);
    });
</script>
// 添加轨迹SVG容器
<svg id="trajectory-viz" width="600" height="400"></svg>

<script>
    const trajectoryData = [
        {x: 50, y: 200},
        {x: 150, y: 180},
        {x: 250, y: 220},
        // 添加实际坐标数据...
    ];

    const line = d3.line()
        .x(d => d.x)
        .y(d => d.y)
        .curve(d3.curveNatural);

    d3.select("#trajectory-viz")
        .append("path")
        .datum(trajectoryData)
        .attr("d", line)
        .attr("stroke", "#2D5D4B")
        .attr("fill", "none");
</script>
