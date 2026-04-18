# Project Archive Design

日期：2026-04-18

## 目标

把旧页面剩余的项目全部接回当前主页，但只作为轻量展示，不与 `Cosoul` 主线竞争注意力。

## 问题

当前已经恢复了 `Selected Work`，但仍然没有覆盖旧页面里的全部项目。用户希望这些项目都能出现，因为它们毕竟也是项目经历。

如果继续把这些内容往 `Selected Work` 里堆，会出现两个问题：

1. 区块层级混乱
2. 补充内容重新抢占主线注意力

## 方案

新增一个更靠后的 `Project Archive` 区块。

### 分层策略

1. `Cosoul`：主轴
2. `Selected Work`：较强补充
3. `Project Archive`：轻量归档展示

## 归档内容

使用旧页面中研究/分析类项目做轻量卡片展示，包括：

1. Avalanche Forecasting
2. Bitcoin Gold Analysis
3. Medical CT Study
4. Medium-Manganese Modeling
5. Olympic Analytics
6. Tennis Analytics

## 设计原则

1. 每个项目只展示一张代表图
2. 每张卡片文案短、轻、信息密度高
3. 不再给这些归档项目做复杂 gallery
4. `FitTrack` 仍然保留在上层，保持“多一丢丢”的权重
