# **户外太阳能自动灌溉系统**

简介：全自动 无人值守灌溉系统
>
> 开源协议: CC-BY-NC-SA 3.0

## 起因

背景故事：从前，老哥在读高一，学校靠近大山，有一大片空地。一天，领导突发奇想，要搞劳动教育，让TJR和他的同学们种菜。TJR看见地里非常干，需要经常浇水，想做一个自动灌溉系统，于是就有了这个项目。

### 外围设备（仅供参考）

1. 带有音乐芯片的功放模块
2. 土壤湿度模块
3. DHT11温湿度探头
4. 大容量蓄电池
5. 大功率太阳能发电板

------



## 功能

1. 每隔30分钟进行一次土壤湿度检测，当达到湿度阈值的探头数大于或等于 启动浇水的最小探头数 则启动浇水程序
2. 浇水前，会放音警告周围人员避让
3. 当浇水时间达到 单次浇水时长 后，自动停止浇水
4. 长时间停留在非主页面（时间页）无操作，自动切换到主页面
5. 长时间无操作，自动熄灭数码管（按菜单键唤醒）

| 菜单编号 | 菜单功能（左2数码管）    | 菜单功能（右2数码管）    |
| -------- | ------------------------ | ------------------------ |
| 主页面   | 当前时间（小时部分）     | 当前时间（分钟部分）     |
| A        | 实时温度（整数部分）     | 实时温度（小数部分）     |
| B        | -                        | 单次浇水时长（分钟）     |
| C        | 禁止浇水开始时间（小时） | 禁止浇水结束时间（小时） |
| D        | 允许浇水最小温度（℃）    | 允许浇水最大温度（℃）    |
| E        | 保存设置                 | 保存设置                 |
| F        | 继电器手动开关           | 继电器手动开关           |
| G        | -                        | 启动浇水的最小探头数     |
| H        | 传感器手动开关           | 传感器手动开关           |

| 按键名称 | 作用                                        |
| -------- | ------------------------------------------- |
| 菜单     | 按下按键，切换下一个菜单 / 唤醒熄灭的数码管 |
| 设置     | 按下按键，进入当前菜单的设置界面            |
| 加       | 按下（支持长按）按键，增加当前数值          |

#### 时间设置方法

1. 上电前按住 设置 键不放，直到系统自检完毕（继电器等关闭）后松手
2. 进入小时设置页面，按 加 键增加小时
3. 按 设置键 进入分钟设置页面， 按 加 键增加分钟
4. 按 设置键 进入保存页面，按 加 键保存时间设置

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/01.jpeg)

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/02.jpeg)

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/03.jpeg)

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/04.jpeg)

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/05.jpeg)

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/06.jpeg)

## 原理图

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/07.png)



## PCB

![](https://github.com/Axuan1226/Outdoor-solar-automatic-irrigation-system/raw/main/img/08.png)
