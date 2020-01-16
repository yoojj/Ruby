# Ruby on Rails
: 웹 애플리케이션을 위한 프레임워크    
: MVC 아키텍처, CoC 패러다임, DRY 원칙 기반     
: 메타프로그래밍에 의존하는 장단점   
: 테스트, 개발, 서비스 3개 환경 제공    


- Puma 웹 서버 기본
- SQLite3 DBMS 기본  



```bash
# 설치
$ gem install rails
$ rails -v

# 생성
$ rails new 프로젝트

# 실행
$ rails server
$ rails s
$ rails s -b 아이피 -p 포트

# 웹 서버 변경
$ rails s thin
$ rails s mongrel
```


## 기본 구조 

```
프로젝트/
├── app/                # MVC, helper 등 실행 파일
├── bin/                # ruby script 실행 파일  
├── config/             # rails, db, routing 등 설정 파일
    └── environments/   # 테스트, 개발, 서비스에 관한 환경 설정
├── db/                 # db 스키마, 마이그레이션 파일
├── lib/          
├── log/
├── public/             # 정적 파일, 공개 파일
├── test/
├── tmp/                # 레일즈가 중간 처리 과정에 사용하는 임시 파일들 저장
├── vender/             # 서드 파티   
├── Gemfile             # gem 의존성 정보 기술
├── Gemfile.lock        # bundler를 위한 gem 버전과 저장소 기술
├── Rakefile            # 빌드, 패키징, 테스드   
├── config.ru           # Rack 설정 파일, 엔트리 포인트  
└── package.json        # rails 5.0 도입  
```



## Rails API  
https://api.rubyonrails.org/


- ActionCable   
- ActionDispatcher
- ActionController
- ActionView
- ActiveResource
- ActionRecord
- ActionJob
- ActionWebService
- ActionMailer
