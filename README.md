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

## 入门指南

### 前置要求

在开始之前，请确保您的系统满足以下要求：

- **Node.js**：版本 18.0 或更高（推荐使用 LTS 版本）
- **包管理器**：npm (随 Node.js 安装) 或 yarn
- **浏览器**：现代浏览器（如 Chrome、Firefox、Edge）
- **钱包**：Freighter Wallet ≥ v5.0.2

### 安装步骤

1. **克隆仓库**
   ```bash
   git clone https://github.com/dvlan26/Crowdfunding-dApp-Demo.git
   cd Crowdfunding-dApp-Demo
   ```

2. **安装依赖**
   ```bash
   npm install
   # 或者使用 yarn
   # yarn install
   ```

   这个步骤会下载所有必要的依赖包，通常需要几分钟时间。

3. **运行开发服务器**
   ```bash
   npm run dev
   # 或者使用 yarn
   # yarn dev
   ```

   服务器将在 http://localhost:3000 启动。您应该会看到类似以下的输出：
   ```
   ready - started server on 0.0.0.0:3000, url: http://localhost:3000
   ```

4. **访问应用**
   
   在浏览器中打开 [http://localhost:3000](http://localhost:3000) 查看应用。

### 配置钱包

5. **安装 Freighter Wallet**
   
   如果尚未安装，请从 [Freighter Wallet 官网](https://www.freighter.app/) 下载并安装浏览器扩展。

6. **启用实验模式**
   
   打开 Freighter Wallet，点击设置（齿轮图标），启用 "Experimental Mode"。

7. **连接网络**
   
   在 Freighter 中选择 Futurenet 网络（或根据需要选择其他网络）。

### 开始使用

8. **连接钱包**
   
   在应用中点击 "Connect Wallet" 按钮，选择 Freighter 钱包进行连接。

9. **Mint 测试代币**
   
   点击 "Mint 100 EXT" 按钮获取示例代币，用于测试捐款功能。

10. **参与众筹**
    
    查看众筹活动详情，输入捐款金额并确认交易。

**注意**：如果页面显示空白或出现 "Account not found" 错误，请确保您的钱包地址已在所选网络上获得资金。

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

# English Version

# Crowdfunding dApp Demo

![Screenshot of the Example Dapp](screenshot.png)

This is a crowdfunding decentralized application (dApp) frontend demo project based on [Next.js](https://nextjs.org/), demonstrating how to build a user interface that connects to smart contracts on the Stellar blockchain. The project showcases the creation of crowdfunding campaigns, fund raising, and user interactions.

## Project Overview

This demo includes the following core features:

- **Wallet Connection**: Supports Freighter wallet connection
- **Account Information**: Displays user balance and account details
- **Crowdfunding Status**: Real-time display of fundraising progress, target amount, and remaining time
- **Fund Deposits**: Allows users to donate to crowdfunding projects
- **Transaction History**: Displays user's deposit records
- **Mint Tokens**: Demo feature allowing users to mint example tokens (EXT)

## Technology Stack

- **Frontend Framework**: Next.js 13+ (React)
- **Styling**: CSS Modules
- **Blockchain**: Stellar (Soroban Contracts)
- **Wallet**: Freighter Wallet

## Getting Started Guide

### Prerequisites

Before starting, ensure your system meets the following requirements:

- **Node.js**: Version 18.0 or higher (LTS version recommended)
- **Package Manager**: npm (installed with Node.js) or yarn
- **Browser**: Modern browser (such as Chrome, Firefox, Edge)
- **Wallet**: Freighter Wallet ≥ v5.0.2

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/dvlan26/Crowdfunding-dApp-Demo.git
   cd Crowdfunding-dApp-Demo
   ```

2. **Install Dependencies**
   ```bash
   npm install
   # or use yarn
   # yarn install
   ```

   This step will download all necessary dependency packages, which usually takes a few minutes.

3. **Run the Development Server**
   ```bash
   npm run dev
   # or use yarn
   # yarn dev
   ```

   The server will start at http://localhost:3000. You should see output similar to:
   ```
   ready - started server on 0.0.0.0:3000, url: http://localhost:3000
   ```

4. **Access the Application**
   
   Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.

### Configure Wallet

5. **Install Freighter Wallet**
   
   If not already installed, download and install the browser extension from the [Freighter Wallet official website](https://www.freighter.app/).

6. **Enable Experimental Mode**
   
   Open Freighter Wallet, click settings (gear icon), and enable "Experimental Mode".

7. **Connect to Network**
   
   In Freighter, select the Futurenet network (or other networks as needed).

### Start Using

8. **Connect Wallet**
   
   In the application, click the "Connect Wallet" button and select Freighter wallet to connect.

9. **Mint Test Tokens**
   
   Click the "Mint 100 EXT" button to obtain example tokens for testing donation functionality.

10. **Participate in Crowdfunding**
    
    View crowdfunding campaign details, enter donation amount, and confirm the transaction.

**Note**: If the page appears blank or shows "Account not found" error, ensure your wallet address is funded on the selected network.

## File Structure

```
/
├── pages/                 # Next.js Pages
│   ├── _app.tsx          # Application Entry
│   └── index.tsx         # Home Page
├── components/            # React Components
│   ├── atoms/            # Basic Components
│   ├── molecules/        # Composite Components
│   └── organisms/        # Page-level Components
├── styles/               # Global Styles
├── public/               # Static Resources
└── assets/               # Icons and Resources
```

## Component Description

### Atoms (Basic Components)
- **AmountInput**: Amount input field
- **AuthorInfo**: Author information display
- **Button**: Generic button
- **Card**: Card container
- **Checkbox**: Checkbox
- **ConnectButton**: Wallet connect button
- **Loading**: Loading indicator
- **ProgressBar**: Progress bar
- **Spacer**: Spacing component

### Molecules (Composite Components)
- **Deposits**: Deposit records list
- **FormPledge**: Donation form
- **TransactionModal**: Transaction confirmation modal
- **WalletData**: Wallet data display

### Organisms (Page-level Components)
- **Campaign**: Crowdfunding campaign details
- **Pledge**: Donation component

## User Workflow

1. **Connect Wallet**
   - Click the "Connect Wallet" button
   - Connect using Freighter wallet
   - Ensure wallet has experimental mode enabled

2. **View Account Information**
   - Display current balance
   - View supported asset types

3. **Participate in Crowdfunding**
   - View campaign target and progress
   - Enter donation amount
   - Confirm transaction

4. **Mint Example Tokens**
   - Use "Mint 100 EXT" button to get test tokens
   - For testing donation functionality

## Demo Screenshot

![Screenshot of the Example Dapp](screenshot.png)

## Notes

- This is a frontend demo project, does not include backend contract deployment
- Requires connection to Stellar network and Soroban RPC
- Freighter wallet is recommended for testing
- Example token (EXT) is for demonstration purposes only

## Related Links

- [Next.js Documentation](https://nextjs.org/docs)
- [Stellar Documentation](https://developers.stellar.org/)
- [Soroban Documentation](https://soroban.stellar.org/)
- [Freighter Wallet](https://www.freighter.app/)

