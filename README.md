# Crowdfunding dApp Demo

![Screenshot of the Example Dapp](screenshot.png)

这是一个基于 [Next.js](https://nextjs.org/) 的众筹去中心化应用 (dApp) 前端演示项目，展示了如何构建连接 Stellar 区块链智能合约的用户界面。该项目演示了众筹活动的创建、资金募集和用户交互功能。

## 项目概述

本 Demo 包含以下核心功能：

- **钱包连接**：支持 Freighter 钱包连接
- **账户信息**：显示用户余额和账户详情
- **众筹状态**：实时显示募集进度、目标金额和剩余时间
- **资金存款**：允许用户向众筹项目捐款
- **交易历史**：展示用户的存款记录
- **Mint 代币**：演示功能，允许用户铸造示例代币 (EXT)

## 技术栈

- **前端框架**：Next.js 13+ (React)
- **样式**：CSS Modules
- **区块链**：Stellar (Soroban 合约)
- **钱包**：Freighter Wallet

## 文件结构

```
/
├── pages/                 # Next.js 页面
│   ├── _app.tsx          # 应用入口
│   └── index.tsx         # 主页
├── components/            # React 组件
│   ├── atoms/            # 基础组件
│   ├── molecules/        # 复合组件
│   └── organisms/        # 页面级组件
├── styles/               # 全局样式
├── public/               # 静态资源
└── assets/               # 图标和资源
```

## 组件说明

### Atoms (基础组件)
- **AmountInput**: 金额输入框
- **AuthorInfo**: 作者信息显示
- **Button**: 通用按钮
- **Card**: 卡片容器
- **Checkbox**: 复选框
- **ConnectButton**: 钱包连接按钮
- **Loading**: 加载指示器
- **ProgressBar**: 进度条
- **Spacer**: 间距组件

### Molecules (复合组件)
- **Deposits**: 存款记录列表
- **FormPledge**: 捐款表单
- **TransactionModal**: 交易确认模态框
- **WalletData**: 钱包数据展示

### Organisms (页面级组件)
- **Campaign**: 众筹活动详情
- **Pledge**: 捐款组件

## 用户工作流

1. **连接钱包**
   - 点击"Connect Wallet"按钮
   - 使用 Freighter 钱包连接
   - 确保钱包已启用实验模式

2. **查看账户信息**
   - 显示当前余额
   - 查看支持的资产类型

3. **参与众筹**
   - 查看活动目标和进度
   - 输入捐款金额
   - 确认交易

4. **Mint 示例代币**
   - 使用"Mint 100 EXT"按钮获取测试代币
   - 用于测试捐款功能

## 演示截图

![Screenshot of the Example Dapp](screenshot.png)

## 注意事项

- 此为前端演示项目，不包含后端合约部署
- 需要连接到 Stellar 网络和 Soroban RPC
- 建议使用 Freighter 钱包进行测试
- 示例代币 (EXT) 仅用于演示目的

## 相关链接

- [Next.js 文档](https://nextjs.org/docs)
- [Stellar 文档](https://developers.stellar.org/)
- [Soroban 文档](https://soroban.stellar.org/)
- [Freighter Wallet](https://www.freighter.app/)
