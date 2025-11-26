## 🚀 Cài đặt và Chạy

### 1. Cài đặt dependencies
```bash
npm install
npm run frontend:install
```

### 2. Khởi động Hardhat local node (terminal 1)
```bash
npm run node
```

### 3. Deploy smart contracts (terminal 2)  
```bash
npm run deploy:local
```

### 4. Khởi động frontend (terminal 3)
```bash
npm run frontend:start
```

Ứng dụng sẽ mở tại `http://localhost:3000`

## 🔧 Cấu hình

Cập nhật địa chỉ contract trong `src/utils/constants.js` sau khi deploy:

```javascript
export const CONTRACT_ADDRESSES = {
  CAMPAIGN_FACTORY: "0x5FbDB2315678afecb367f032d93F642f64180aa3" // Thay bằng địa chỉ thực
};
```

## Tạo Custom Network trong MetaMask
Để kết nối MetaMask với Hardhat local node, bạn cần tạo một Custom Network trong MetaMask với các thông tin sau:
- **Network Name**: Hardhat Localhost
- **New RPC URL**: http://127.0.0.1:8545
- **Chain ID**: 31337
- **Currency Symbol**: ETH
--
---
-----
