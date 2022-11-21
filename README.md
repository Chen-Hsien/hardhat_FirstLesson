# hardhat_FirstLesson

Hardhat是開發測試智能合約其中一種好用的開發工具，其他還有Truffle Vs Remix，在搜集資料中這篇文章很好的比較了三者的優缺點[Compare](https://theblockchainguy.dev/hardhat-vs-truffle-vs-remix)根據自身的狀況來挑選開發工具吧～.  

### 創建專案

以下使用環境為MacOS->Terminal.  
```CLI
mkdir hardhat-practice
cd hardhat-practice
npm init --yes
npm install --save-dev hardhat
```

安裝完後在hardhat-practice下執行hardhat起來.  
```CLI
npx hardhat
```
<img width="570" alt="image" src="https://user-images.githubusercontent.com/24216536/202661522-1e3502d1-d404-4ef1-8be7-33f7d0b8a547.png">   

下面有四個選項，方便一步步了解hardhat架構，從Create an empty hardhat.config.js開始.  
選擇後會在資料夾下建立`hardhat.config.js` 文件，未來對Hardhat的控制就從這個config修改.  

### Hardhat 架構
Hardhat依照官方文件提供的服務主要以[Task](https://hardhat.org/hardhat-runner/plugins),[Plugin](https://hardhat.org/hardhat-runner/plugins)的方式，可以自由選擇想要執行的Task以及使用的Plugin.   

#### Task
<img width="646" alt="image" src="https://user-images.githubusercontent.com/24216536/202893318-af6486b4-45ab-450a-8631-ea901edf5fa0.png">.  
並從CLI選擇想要執行的Hardhat任務。  

#### Plugin
hardhat 最著名的套件是
Ethers.js（Web3.js 的另一個選擇）   
可與錢包、帳戶、合約互動的各種功能，以及ABICoder, BigNumber, HDNode, address等常用功能的集合。   
Waffle（Truffle 測試工具的另一個選擇）
為TypeScript原生，並設計用來和Ethers搭配，可以很好的用於以太坊地址, Hash, BigNumbers的Chai斷言庫   

#### 練習正文開始
Create an empty hardhat.config.js後會得到如下的設定檔
```Solidity
/** @type import('hardhat/config').HardhatUserConfig */
module.exports = {
  solidity: "0.8.17",
};
```







從CLI執行Hardhat
