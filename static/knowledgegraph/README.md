# 知识图谱相关

python 测试代码，并没有工程化到 patroit 平台中

## 文件说明

+ `kg_preprocessing.py` 知识图谱预处理
+ `rp_preprocessing.py` 针对电商大类的预处理

## 知识图谱建立

目前是人工操作，之后需要大批量建立的时候，则会采取自动 + 人工干预的方法。按照目前的技术水平，基本可以说离不开人工干预。

+ 调研图数据库

## 图谱保存格式

按照不同的分类保存，分为 

+ `2tier`: 二级类目
+ `3tier`: 三级类目
+ `4tier`: 四级类目
+ `5tier`: 五级类目

每个类别的存储为 TXT 文档，按照行来分类，格式为：

```
第一行 - 节点名称：技术 工程技术
第二行 - 父节点名称（可以有多个）：总分类
第三行 - 子节点名称：媒体技术 医学 技术导航模板 技术标志 航空航天 专利 园艺技术 制造 数位技术 技术小作品 工业设计 通信技术 技术预测 各类技术 技术系统 TED 计算机技术 技术通信 发明 纺织 技术变革 核能科技 技术模板 家政学 能源 产业 技术网站 建筑 技术大学和学院 生产 互联网 电信技术 技术总论 科技产品 高新技术 技术民俗学 技术史 农业 无线 复健医学 印刷
第四行 - 暂无：None
第五行 - 暂无：None
```