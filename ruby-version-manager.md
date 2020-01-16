# ruby version manager

- [rvm](#rvm)
- [rbenv](#rbenv)



## rvm

```bash
# 설치
$ sudo yum install curl gpg gnupg2

## 싱글 유저
$ curl -sSL https://get.rvm.io | bash -s stable
$ source ~/.rvm/scripts/rvm

## 멀티 유저
$ curl -sSL https://get.rvm.io | sudo bash -s stable
$ source /etc/profile.d/rvm.sh


# 확인
$ rvm -v


# 제거
$ rvm implode
$ gem uninstall rvm


# 루비 설치
$ rvm install 버전

# 특정 버전 사용
$ rvm use 버전

# 루비 제거
$ rvm remove 버전

# 확인
$ rvm list
$ ruby -v
```



## rbenv

```bash
# 설치
$ git clone git://github.com/sstephenson/rbenv.git ~/.rbenv

## 환경 변수 등록
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
$ source ~/.bashrc

#$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
#$ echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
#$ source ~/.bash_profile


# 확인
$ rbenv -v
```
