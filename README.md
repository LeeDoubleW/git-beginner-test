# Hello, I'm LeeDoubleW!
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 🔥 Working Hard!!

![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

sequenceDiagram
    participant ProductController
    participant ProductService
    participant ProductRepository
    ProductController->>+ProductService:상품조회요청
    alt 상품ID O
    ProductService->>+ProductRepository:getProductInfo()
    ProductRepository-->>ProductService:해당 상품 정보
    else 상품ID X
    ProductService->>+ProductRepository:getProductListInfo()
    ProductRepository-->>-ProductService:상품 목록
    end
    ProductService-->>ProductController: 요청 정보 전달
