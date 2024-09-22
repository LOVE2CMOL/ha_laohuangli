
### 中国老黄历 (Chinese Almanac) for Home Assistant

"中国老黄历"是一个为Home Assistant设计的自定义组件，旨在为您的智能家居带来传统中国历法的智慧。这个插件提供丰富的中国传统历法信息，包括农历日期、节气、吉凶宜忌等，让您在现代智能家居系统中感受传统文化的魅力。

## 功能
显示当前日期的农历信息，提供二十四节气信息，显示每日吉凶、宜忌，实时更新时辰凶吉信息，展示生肖、星座等个人信息，提供传统节日提醒，支持自定义更新频率。

## 安装
1. 将`custom_components/chinese_almanac`文件夹复制到您的Home Assistant配置目录下的`custom_components`文件夹中。
2. 重启您的Home Assistant。
3. 在集成页面中搜索"中国老黄历"并添加集成。

## 可用传感器
安装后，您将获得以下传感器：日期、农历、星期、今日节日、八字、今日节气、下一节气、季节、时辰凶吉、生肖冲煞、星座、星次、彭祖百忌、十二神、廿八宿、今日三合、今日六合、纳音、九宫飞星、吉神方位、今日胎神、今日吉神、今日凶煞、宜忌等第、宜、忌、时辰经络。

## 使用
安装并配置后，您可以在Home Assistant的仪表板中添加这些传感器。例如，创建一个卡片来显示今天的农历日期和宜忌信息：

```yaml
type: entities
entities:
  - entity: sensor.老黄历_农历
  - entity: sensor.老黄历_宜
  - entity: sensor.老黄历_忌
```

## 致谢
本项目使用了[cnlunar](https://github.com/6tail/lunar-python)库来计算农历信息，在此表示感谢。