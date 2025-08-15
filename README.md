# Dear_Carmate 개인 개발 리포트

## 1. 📑프로젝트 개요
-  Dear Carmate는 중고차 딜러들이 사용하는 중고차 계약 관리 서비스입니다. 차량과 고객, 계약 관리에 특화된 서비스를 제공하여 사용자의 업무 효율을 높이고, 매출 분석까지 가능합니다.
-  프로젝트 기간: 2025.07.22~2025.08.13
-  주요 기능: auth API/ user API/ company API/ car API/ customer API/ contract API/ contract-document API/ image API/ dashboard API
---
## 2. ⚙️ 기술 스택

<h3 align="center"><b>📚 Languages 📚</b></h3>

<p align="center"> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" /> 
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" /> </p>

<h3 align="center"><b>⚙️ Frameworks & Libraries</b></h3>

<p align="center"> <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" /> <img src="https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white" /><br/>  <img src="https://img.shields.io/badge/Passport-34E27A?style=for-the-badge&logo=passport&logoColor=white" /> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" /> <img src="https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white" /> <img src="https://img.shields.io/badge/Prettier-F7B93E?style=for-the-badge&logo=prettier&logoColor=black" /> </p>

<h3 align="center"><b>🗄️ Database & Hosting</b></h3>

<p align="center"> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" /> <img src="https://img.shields.io/badge/Render-0099E5?style=for-the-badge&logo=render&logoColor=white" /> </p>

<h3 align="center"><b>🔧 Development Tools </b></h3>

<p align="center"> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /> <img src="https://img.shields.io/badge/Nodemon-76D04B?style=for-the-badge&logo=nodemon&logoColor=white" /> <img src="https://img.shields.io/badge/TS Node-3178C6?style=for-the-badge&logo=ts-node&logoColor=white" /> <img src="https://img.shields.io/badge/Dotenv-ECD53F?style=for-the-badge&logo=dotenv&logoColor=black" /> </p>


<h3 align="center"><b>🔐 Authentication & Utility Libraries </b></h3>
<p align="center">
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white" alt="JWT" />
  <img src="https://img.shields.io/badge/Nodemailer-009966?style=for-the-badge&logo=gmail&logoColor=white" alt="Nodemailer" />
  <img src="https://img.shields.io/badge/Multer-1E90FF?style=for-the-badge&logo=files&logoColor=white" alt="Multer" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
</p>

<h3 align="center"><b> 🤝 Collaboration Tools </b></h3>
<p align="center"> <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white" alt="Notion" /> <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /> <img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /> </p>

---
## 3. 👓담당 작업 
### 1. Company API
: 어드민만 접근할 수 있는 페이지로 회사 목록/ 회사별 유저 목록 조회 가능 

: 어드민만 접근할 수 있도록 authorizeAdmin 미들웨어 코드를 추가함
- 회사 등록
- 회사 목록 조회
- 회사별 유저 조회
- 회사 수정
- 회사 삭제

### 2. Car API
: 해당 회사의 차량만 조회/ 수정/ 삭제 가능하도록 구현

: 프론트엔드와의 연동을 위해 converter.ts 파일 추가 
- 차량 등록
- 차량 목록 조회
- 차량 수정
- 차량 삭제
- 차량 상세 정보 조회
- 차량 데이터 대용량 업로드
- 차량 모델 목록 조회

### 3. 그 외
- firebase 연결
  - firebase storage 생성
  - firebase-admin.ts 작성
 
---
## 4. 🖥️ 기능 구현 예시
### 회사 등록
: 어드민 계정은 회사이름과 코드를 입력하여 회사 등록 가능
<img width="1195" height="583" alt="회사 생성" src="https://github.com/user-attachments/assets/5916aae0-d029-4c57-8b83-415ca0e94966" />

### 회사 목록 조회 
: 어드민 계정은 회사 목록 조회가 가능하며, 페이지네이션과 검색 기능 가능함
#### 목록 조회
<img width="1188" height="776" alt="컴패니 조회" src="https://github.com/user-attachments/assets/e7163190-cf1a-4bec-b52a-e22263785579" />

#### 페이지네이션
<img width="1192" height="771" alt="회사 페이지네이션" src="https://github.com/user-attachments/assets/7c4e62a8-a306-46b7-9d21-1009a3ffb532" />

#### 회사이름 검색
<img width="1191" height="686" alt="회사 검색 가능" src="https://github.com/user-attachments/assets/ed6a015f-2d52-433d-93ff-e5c4ca36f4c0" />


### 회사별 유저 조회
: 어드민 계정은 유저 목록 조회가 가능하며, 페이지네이션과 검색 기능 가능함
#### 목록 조회
<img width="1188" height="780" alt="유저 조회" src="https://github.com/user-attachments/assets/a664afa3-9d05-42cb-a472-5c3df21b02b6" />

#### 페이지네이션
<img width="1181" height="768" alt="유저 페이지네이션" src="https://github.com/user-attachments/assets/7bd7f00e-ea38-462f-92a2-21df3977944d" />

#### 직원이름 검색
<img width="1159" height="766" alt="유저 이름 검색" src="https://github.com/user-attachments/assets/f121b6bc-0f1c-40a8-8074-23d7f01ea53c" />

### 회사 수정
<img width="1188" height="592" alt="회사 수정" src="https://github.com/user-attachments/assets/6c4e142d-52e5-484d-ab1f-06006bb0538e" />

### 회사 삭제
<img width="1189" height="552" alt="회사 삭제" src="https://github.com/user-attachments/assets/d7b80b07-d526-4104-9c44-3b544fb8001c" />


### 차량 등록
: status는 기본값 등록
<img width="1197" height="756" alt="차량 생성" src="https://github.com/user-attachments/assets/8de61922-325a-48b2-bfe0-a906e95c884b" />

### 차량 목록 조회
: 회사에 속한 차량 조회 가능하며 페이지네이션과 검색 기능 가능함
#### 목록 조회
<img width="1151" height="814" alt="차량 조회" src="https://github.com/user-attachments/assets/bd4bb295-8267-4b84-b26c-df7114fe181e" />

### 페이지네이션
<img width="1485" height="789" alt="get 페이지네이션2" src="https://github.com/user-attachments/assets/23580e82-6bce-476c-bef8-53926100529b" />

### 차량번호 검색
<img width="1188" height="775" alt="차량번호페이지네이션" src="https://github.com/user-attachments/assets/baf28831-7949-41f2-936d-76496509e0c8" />

### 차량 수정
<img width="1466" height="736" alt="patch" src="https://github.com/user-attachments/assets/fea463b9-d2c2-48ea-a804-67d9f5fd1194" />

### 차량 삭제
<img width="1483" height="532" alt="delete" src="https://github.com/user-attachments/assets/a662c19d-2f83-44cd-9365-a33bb3f19488" />

### 차량 상세 조회
<img width="1487" height="496" alt="get 상세조회" src="https://github.com/user-attachments/assets/dfcdba1f-2bce-40c9-9602-fe6480433510" />

### 차량별 모델 조회
<img width="1193" height="774" alt="차량별 모델 조회" src="https://github.com/user-attachments/assets/fe3387f7-21aa-4fec-a334-50cd0d946d7c" />

### csv 대용량 업로드 
<img width="1486" height="467" alt="csv 업로드 테스트" src="https://github.com/user-attachments/assets/2675187d-133d-4b59-a4be-7a6914a794c6" />

### authorizeAdmin 코드 추가 
: company API의 경우 관리자만 접속 가능한 페이지이기 때문에 관리자인지 확인하는 코드를 추가함
```
export const authorizeAdmin = (req: AuthRequest, res: Response, next: NextFunction): void => {
  if (!req.user) {
    res.status(401).json({ message: '로그인이 필요합니다.' });
    return;
  }
  // 관리자 권한 확인
  if (req.user.isAdmin) {
    next();
  } else {
    res.status(403).json({ message: '관리자 권한이 필요합니다' });
  }
};
```
```
const CompaniesRouter = (prisma: PrismaClient): Router => {
  const router = Router();

  const companyRepository = new CompanyRepository(prisma);
  const companyService = new CompanyService(companyRepository);
  const companyController = new CompanyController(companyService);

  router.use(isAuthenticated);
  router.use(authorizeAdmin);
.
.
.
```

### Firebase admin sdk 초기화 코드 작성
: Firebase storage 생성 후 firebase-admin.ts 파일 작성
- **Node.js같은 서버 환경에서는 Firebase의 모든 기능을 관리자 권한으로 사용하기 위해 Firebase Admin SDK 초기화 과정이 필요함**
```
import * as admin from 'firebase-admin';

// 환경 변수에서 서비스 계정 키를 읽어옵니다.
const privateKey = process.env.FIREBASE_PRIVATE_KEY;
const clientEmail = process.env.FIREBASE_CLIENT_EMAIL;
const projectId = process.env.FIREBASE_PROJECT_ID;
const storageBucket = process.env.FIREBASE_STORAGE_BUCKET;

// 환경 변수가 모두 설정되었는지 확인
if (!privateKey || !clientEmail || !projectId || !storageBucket) {
  throw new Error('Firebase environment variables are not all set.');
}

if (!admin.apps.length) {
  admin.initializeApp({
    credential: admin.credential.cert({
      projectId,
      clientEmail,
      privateKey: privateKey.replace(/\\n/g, '\n'), // 개행 문자 처리
    }),
    storageBucket,
  });
}

export default admin;
```

1) process.env를 통해 .env에 설정된 서비스 계정 정보를 가져옴
2) if문을 통해 환경변수가 모두 존재하는지 확인하며, 하나라도 없을 시에는 Error를 발생시킴
3) admin.credential.cert() 함수를 사용하여 Firebase 서비스 계정 키를 인증 정보로 변환
4) admin.initializeApp() 함수를 호출하여 Firebase Admin SDK를 초기화


---
## 5. 🗒️문제점 및 해결 과정
### 프론트엔드와의 연동 문제 
: 프론트엔드로 지정되어 있는 값과, responses의 값이 달라 프론트엔드에서 값이 보이지 않는 오류
- 문제 확인 과정
1) 스키마 설정에서 map을 통해 프론트엔드에서 지정한 enum값 (possession,contractProceeding, contractCompleted)과 동일하게 데이터베이스에 저장
2) 프론트엔드 연동 테스트에서 차량 status 값이 나오지 않는 것을 확인하게 됨
3) console.log를 통해 확인해보니 responses가 (POSSESSION, CONTRACT_PROCEEDING, CONTRACT_COMPLETED)로 나오는 것을 확인함
4) 매핑 코드를 작성하여 responses로 지정되어 있는 enum을 동일하게 맞춰줌
 
- 문제 해결 방법
1) car.converter.ts 파일 작성
```
import { CarStatus, CarType } from '@prisma/client';

/**
 * CarStatus Enum을 camelCase로 변환
 */
export function carStatusToCamelCase(status: CarStatus | null): string | null {
  if (!status) return null;

  const statusMapping: Record<CarStatus, string> = {
    [CarStatus.POSSESSION]: 'possession',
    [CarStatus.CONTRACT_PROCEEDING]: 'contractProceeding',
    [CarStatus.CONTRACT_COMPLETED]: 'contractCompleted',
  };

  return statusMapping[status] || status;
}

/**
 * CarType Enum을 한글로 변환
 */
export function carTypeToKorean(type: CarType | null): string | null {
  if (!type) return null;

  const typeMapping: Record<CarType, string> = {
    [CarType.COMPACT]: '경·소형',
    [CarType.MIDSIZE]: '준중·중형',
    [CarType.FULLSIZE]: '대형',
    [CarType.SPORTS]: '스포츠카',
    [CarType.SUV]: 'SUV',
  };

  return typeMapping[type] || type;
}

/**
 * Car 엔티티의 enum 필드들을 변환
 */
export function convertCarEnums(car: { status: CarStatus | null; type: CarType | null }) {
  return {
    status: carStatusToCamelCase(car.status),
    type: carTypeToKorean(car.type),
  };
}

```

2) return에 반영
```
  return {
      id: newCar.id,
      carNumber: newCar.carNumber,
      manufacturer: newCar.manufacturer,
      model: newCar.model,
      type: carTypeToKorean(newCar.type) as CarType,
      manufacturingYear: newCar.manufacturingYear,
      mileage: newCar.mileage,
      price: newCar.price.toNumber(),
      accidentCount: newCar.accidentCount,
      explanation: newCar.explanation,
      accidentDetails: newCar.accidentDetails,
      status: carStatusToCamelCase(newCar.status) as CarStatus,
    };
```

### 페이지네이션 오류 
: findMany 함수에 페이지네이션을 위한 take와 skip인자가 올바르게 전달되지 않아 발생한 오류 
- 문제 확인 과정
1) get API 테스트 시 에러 발생
```
[ERROR] 
Invalid `this.prisma.car.findMany()` invocation in
/home/yun-heewon/Dear_Carmate_be/src/cars/repository.ts:35:28

  32 }
  33 
  34 async findManyCar(options: FindManyCarOptions) {
→ 35   return this.prisma.car.findMany({
         skip: NaN,
         where: {
           companyId: 166
         },
         orderBy: {
           id: "asc"
         },
       + take: Int
       })

Argument `take` is missing.
```
2) take 인자 누락과 skip 인자로 NaN이 전달됨을 확인
3) 데이터가 문자열인 상태 그대로 Prisma 쿼리에 사용되었고, 컨트롤러에서 실제로 문자열을 숫자로 변환하는 과정이 생략됨.
4) get API 테스트 시 쿼리로 page와 pageSize를 작성해주면 오류가 나지 않고, 프론트엔드에서는 제대로 작동하나 쿼리를 넣어주지 않아도 동작하도록 코드 수정

- 문제 해결 방법
: plainToTinstance 사용하여 타입을 변환

```
getCarList = async (req: Request, res: Response, next: NextFunction) => {
    try {
      const query: CarListQueryDto = req.query as unknown as CarListQueryDto;
      const companyId = req.user?.companyId;

      if (!companyId) {
        return res.status(401).json({ message: '인증되지 않은 사용자입니다.' });
      }
      const carList = await this.carService.getCarList(query, companyId);
      return res.status(200).json(carList);
    } catch (error) {
      return next(error);
    }
  };

                                ↓

getCarList = async (req: Request, res: Response, next: NextFunction) => {
    try {
      const query = plainToInstance(CarListQueryDto, req.query);
      const companyId = req.user?.companyId;

      if (!companyId) {
        return res.status(401).json({ message: '인증되지 않은 사용자입니다.' });
      }
      const carList = await this.carService.getCarList(query, companyId);
      return res.status(200).json(carList);
    } catch (error) {
      return next(error);
    }
  };
```
- const query: CarListQueryDto = req.query as unknown as CarListQueryDto; 를 const query = plainToInstance(CarListQueryDto, req.query); 로 코드 변경
- plainToTnstance의 역할
  : 기존 코드는 타입스크립트 객체에게 Dto 타입이 맞다고 속이는 코드로 작동, **plainToInstance를 통해 Dto에 정의된 데코레이터를 읽고 문자열을 숫자열로 변환해줌**

  
---
## 6. 👥협업 및 코드리뷰
### 데일리 스크럼 진행
- 매일 아침 issue 탭에서 todo 생성 후 데일리 스크럼 진행
- 데일리스크럼은 <어제 한 일, 오늘 할 일, 그 외 논의사항>로 진행함
- issue 탭에 데일리스크럼 정리

### 코드리뷰
- pr 생성 후 작성한 코드와 연관이 있는 사람을 코드리뷰어로 등록
- 리뷰 후 코드 수정 과정을 반복
- 리뷰어의 approve시 pr을 올린 본인이 직접 merge

#### 코드 리뷰어를 하며 알게 된 점 
- **.bind**는 컨트롤러 메소드 정의에 따라 사용될 수 있고, 사용되지 않을 수도 있음.
  - 컨트롤러를 화살표함수로 작성한 경우 this 컨텍스트를 자신이 선언될 때의 스코프에서 정적으로 바인딩함
  - 화살표 함수로 정의하면 항상 해당 클래스의 인스턴스를 가리키게 되어 bind 사용이 필요하지 않음
  - 화살표함수를 작성하지 않은 경우에는 this 컨텍스트를 고정시키는 과정이 필요하기 때문에 .bind 사용이 필요함
    
- **의존성 직성 생성과 주입의 차이**
1) 의존성 직접 생성
     - 객체가 자신의 내부에서 필요한 다른 객체를 직접 만드는 방식
```
import { CarService } from './car.service';

export default class CarController {
  private readonly carService: CarService;

  constructor() {
    this.carService = new CarService(); // CarController가 직접 CarService를 생성
  }
}
.
.
.
```
2) 의존성 주입
     - 외부에서 객체가 필요로 하는 의존성을 주입(Injection)받는 방식

  ```
  export default class CarController {
  private readonly carService: CarService;

  constructor(carService: CarService) {
    this.carService = carService;
  }
  .
  .
  ```

    
| 구분 | 의존성 직접 생성 | 의존성 주입 |
| :--- | :--- | :--- |
| 의존성 획득 방식 | 객체 내부에서 직접 new 키워드로 생성 | 외부에서 객체를 주입받음 |
| 결합도 | 강한 결합 | 느슨한 결합 |
| 유연성 | 낮음(의존성 변경 시 코드 수정 필요함 | 높음(외부에서 주입되는 객체만 변경|
|테스트 용이성| 낮음(mock주입이 어려움) | 높음 |
|재사용성| 낮음| 높음|

---
## 7. ⭐코드 품질 및 최적화 
1) tsconfig 설정을 통한 까다로운 타입 설정
- 타입스크립트의 엄격한 타입 체크 기능을 활용하여 코드의 안정성과 예측 가능성을 높임.
2) class-validator 라이브러리 사용을 통한 dto 설정으로 타입 안정성 확보
- 클래스 기반의 DTO를 정의하고 데코레이터를 사용하여 API 요청 데이터의 유효성을 자동으로 검증하고, 잘못된 형식의 데이터가 비즈니스 로직으로 전달되는 것을 방지함.
3) 의존성 주입 방식으로 클래스를 생성하여 높은 유영성과 테스트 용이성 확보
- 의존성을 외부에서 주입받는 방식을 채택하여 클래스 간의 결합도를 낮추고 코드의 재사용성을 높임. 또한 모의 객체를 주입하여 단위 테스트를 독립적으로 쉽게 수행함.
4) 레이어드 아키텍쳐 설계를 통한 관심사 분리와 유지보수 용이성 확보
- 레포지토리, 서비스, 컨트롤러 층으로 분리하여 각 계층의 역할과 책임을 명확히 함. 관심사 분리를 통해 특정 기능 변경 시 다른 계층에 미치는 영향을 최소화하고 시스템의 유지보수성을 높임. 

---

## 8. 📋향후 개선 사항 및 제안
- 관리자가 회원 탈퇴 및 회사 삭제를 진행할 때 확인 진행
  - 현재 회원 삭제와 회사 삭제 시에는 버튼 한번으로 삭제가 진행되고 있음. 확인을 위해 관리자가 비밀번호를 입력하거나, 경고 메세지 창을 띄우는 등 추가 확인 작업이 있으면 좋을 거 같음.
- 차량 등록 시 제조사 및 차종에 대한 데이터 설정
  - 현재는 회사에 등록되어 있는 제조사와 차종을 선택하여 차량 등록이 가능한 상태임. 직접 입력할 수 있도록 하거나, 외부 데이터를 연동하거나, 프론트엔드에서도 차종을 추가하는 기능을 도입하면 좋을 거 같음.
 
---
## 9. 🪄 이번 팀 프로젝트에 대한 셀프 평가 및 느낀점
- 팀장으로서 pm의 역할을 했어야 했는데 해당 부분은 생각하지 못해 팀 프로젝트 스케줄에 차질이 생김.
  - 이후에는 팀 프로젝트를 시간 안에 끝내기 위해 스케줄 정리를 확실히 해야겠다고 느낌.
- 이번 팀 프로젝트로 코드리뷰를 처음 진행하게 되었는데 코드 작성에 익숙하지 않고, 읽는 것에도 익숙하지 않아 다른 사람이 쓴 코드를 읽는 데 시간이 오래 걸림. 또한 맞게 코드리뷰를 진행했는지 끊임없이 의문이 들게 됨.
  - 더 많은 코드를 접해보고 다양한 코드 스타일들을 경험해봐야 겠다고 느낌.
- 타입스크립트 추가 학습 필요
  - 이번 프로젝트에는 타입스크립트를 사용하여 개발을 진행하였으나 아직도 타입스크립트에 대해 어려움을 느낌. 제네릭 등이 사용되는 코드를 잘 이해하지 못하고, 이해하지 못한 상태로 사용하게 되어 이 부분에 대한 추가학습이 필요하다고 생각됨  

 
