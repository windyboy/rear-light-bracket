# 自行车尾灯支架

用于设计和 3D 打印自行车尾灯支架的模型项目。使用 Autodesk Fusion 编辑模型，并导出 STL 用于切片打印；本项目没有应用代码或自动化测试套件。

## 模型文件

| 文件 | 用途 |
| --- | --- |
| [bicycle_rear_bracker_sample.stl](bicycle_rear_bracker_sample.stl) | 原始参考模型，保留原文件及其现有拼写。 |
| [bicycle_rear_bracket_current.f3d](bicycle_rear_bracket_current.f3d) | 最新版可编辑 Fusion 模型。 |
| [bicycle_rear_bracket_current.stl](bicycle_rear_bracket_current.stl) | 对应的最新版打印模型。 |

## 使用方法

1. 在 Autodesk Fusion 中打开 `bicycle_rear_bracket_current.f3d`，查看或修改设计。
2. 将 `bicycle_rear_bracket_current.stl` 导入切片软件，确认尺寸与方向，按实际材料和打印机设置打印参数。
3. 打印后检查支架与尾灯、自行车安装位置的实际配合。

设计尺寸使用 **mm**。STL 不携带单位信息，导入切片软件时应按毫米解释并核对尺寸。本项目尚未记录推荐材料、打印方向或切片参数。

## 修改与保存

- 关键尺寸使用命名参数和表达式，保留可编辑特征历史。
- 明确孔径、孔间距、方向和贯穿深度；区分孔中心距与内壁净距。
- 默认保留单一实体，将整体包围盒中心对齐原点，连接部分不侵入底座凹槽。
- 修改后检查实际尺寸、孔位、实体连通性和特征错误，并查看模型截图。
- 保存时同步更新两个 `current` 文件，确认 F3D 归档完整、STL 数据有效；保留原始参考模型。
- 临时文件放在 `/tmp` 或 Windows 临时目录，避免在项目中累积中间版本。

CAD 验证不能替代实际装配或打印测试。供自动化建模使用的详细约定见 [AGENTS.md](AGENTS.md)。
