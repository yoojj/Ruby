# ruby gem


- [Gem](#gem)
    - [.gemspec](#.gemspec)
- RubyGems
- Bundler
    - Gemfile


```bash
# 설치 확인
$ gem -v
$ bundle -v
```



## Gem
: 루비 패키지   


**gem 구성**  
- 루비 코드 파일 (*.rb)
- 정보를 제공하는 특수 파일 (.gemspec)
- 일부 패키지에는 성능 향상을 위해 ruby c 파일 존재



### .gemspec
: gem에 대한 정보를 제공하는 파일   


**.gemspec 구성**  
- gem 이름
- gem 버전
- gem 짧은 설명
- gem 의존성 목록
- gem 작성자 정보들


```ex
Gem::Specification.new do |s|
    s.name        = ""
    s.version     = ""
    s.licenses    = ['MIT']
    s.summary     = ""
    s.description = ""
end
```


## RubyGems
: gem 패키지 매니저


명령어 | 설명
---|---
env            | gem 환경 정보 확인
list           | 설치된 패키지 목록 확인
search [name]  | rubygems.org 에서 패키지 검색  
install [name] | 패키지 설치
install [name] -v [version] | 특정 버전 패키지 설치  
which [name]   | 설치한 패키지 위치 확인  
cleanup        | 오래된 패키지 제거

https://guides.rubygems.org/command-reference/



## Bundler
: gem 의존성 관리 도구   
: Gemfile을 이용해 의존성 관리   



### Gemfile  
: gem 의존성이 선언된 파일  


```ex
ruby '0.0.0'

gem 'rails', '~> 0.0.0'
gem 'puma', '~> 0.0.0'
gem 'sqlite3'
```
