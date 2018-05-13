# 架构

![Architecture](https://www.lucidchart.com/publicSegments/view/55b4c3c8-f456-44a4-8283-83b5f0220a1c/image.png)

# 设计

- [x] 思考项目定位和用户故事
- [x] 思考和调研关键技术
- [x] 写开题报告
- [x] 绘制架构图

# 开发

## APP代码拆分与动态链接技术

- [x] 通过npm shrinkwrap来获得APP的依赖和其版本
- [x] 把依赖项打成单独的包
- [x] 去掉原本APP包中依赖项的代码
- [x] 在APP运行时动态链接依赖项
- [x] webpack插件，一键完成这些工作并生成tar.gz包
- [ ] 在较大的项目中尝试使用这种技术，确保稳定性

## 后端开发 (2天)

- [x] 中央服务器接受新APP上传
- [x] 中央服务器管理APP内支付
- [x] 中央APP仓库，管理APP、APP版本数据
- [x] 中央APP仓库，管理APP依赖项
- [x] 中央APP仓库，提供文件下载能力
- [x] 中央APP仓库，提供根据GPS位置发现APP
- [x] 镜像APP仓库（城市CDN或NAT内），提供根据列表发现APP
- [x] 镜像APP仓库和中央APP仓库的同步工具
- [ ] 使用DNS解析的方法让用户就近选择APP仓库
- [ ] docker部署（自动设置间隔时间进行mirror）


## 安卓客户端 (2天)

- [x] 在本地管理依赖库
- [x] APP的logo显示、版本显示、界面修缮
- [x] 在本地拼装与执行APP
- [x] fork cordova来提供native接口调用（如扫码、GPS等能力）
- [x] 调用根据GPS坐标发现APP的接口、在NAT内部发现APP列表
- [x] 一键启动APP的桌面小工具
- [x] 用户信息管理和授权给APP
- [x] 通过签名来实现APP内支付授权
- [x] 带参数地启动一个APP

## DEMO APP开发 (1天)

- [x] 停车场缴费
- [ ] 餐厅点菜
- [ ] 校车时刻表
- [ ] 活动报名

## 其他

- [x] PC端开发体验的api shim
- [ ] 部署和调试
- [ ] 局域网dnsmasq实验

## 部署、论文和答辩 (3天)

- [ ] 论文书写
- [ ] 性能分析（字节传输数）
- [ ] PPT

## Optional roadmap
- [ ] 管理APP已授权信息，即一次授权后后续不再弹出授权

## 时间安排
- [x] APP内支付 + 停车场缴费DEMO APP （1天）
- [x] APP界面、桌面小工具、NAT （1天）
- [ ] 餐厅点菜、校车时刻表、活动报名APP （1天）
- [ ] 局域网内dnsmasq、docker、部署、线路优选 （1.5天）
- [ ] 论文书写和PPT （3天）
