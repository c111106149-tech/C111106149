# 📘 BookSwap 二手書平台 DFD（無交易功能）

```mermaid
flowchart TD
    %% 系統名稱
    System(["BookSwap 二手書平台系統"])

    %% 外部實體
    User(["使用者"])
    Admin(["平台管理者"])

    %% 資料流
    User -->|"註冊 / 登入資料"| System
    User -->|"上傳書籍資訊"| System
    User -->|"交換 / 借閱申請"| System
    System -->|"書籍清單 / 搜尋結果"| User
    System -->|"通知 / 申請回覆"| User

    Admin -->|"登入 / 審核資料"| System
    System -->|"管理報表 / 平台資訊"| Admin
