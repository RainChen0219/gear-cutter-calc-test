# 配刀参数计算器（测试版）

![testing](https://img.shields.io/badge/testing-v1.1.1-orange) ![html](https://img.shields.io/badge/html-100%25-orange)

本仓库为「配刀参数」测试版，用于新功能先行验证，内容可能领先正式版；正式版仓库见 [gear-cutter-calc](https://github.com/RainChen0219/gear-cutter-calc)。

## 在线使用

- GitHub Pages（测试）: https://rainchen0219.github.io/gear-cutter-calc-test/
- jsDelivr CDN（测试）: https://cdn.jsdelivr.net/gh/RainChen0219/gear-cutter-calc-test@main/index.html

## 功能

- 拍照识图自动填写（Beta）：相机拍照或相册选图，自动识别 18 个字段，以橙色待确认填入，人工核对采纳后再计算
- 公制模数 / 英制径节（DP）双模式
- 20° / 25° / 30° 三种压力角
- 内齿/内花键、外齿/外花键
- 加工方式「滚刀」分支（v1.1.1）：外直齿轮/外花键滚刀加工，输出工件参数、公法线与跨棒距、根切校验、滚刀配对、花键大小径；内齿禁用滚刀
- 碗形插齿刀（φ50/φ75/φ100/φ125）、盘形插齿刀（φ160/φ200）自动选型
- 大径/小径/齿厚/量棒距 M/公法线 Wk 智能软填充
- 包络法刀坯计算、x₀ 许用区间推荐
- 五用例回归校验通过

## 使用

直接用浏览器打开 `index.html` 即可，无需安装任何依赖。

## 技术栈

单文件 HTML + 原生 JS + CSS，无外部依赖。拍照识图由后端服务 `https://api.jingmeicuttingtool.com` 提供，模型密钥不暴露在前端。
