## git

---

# 동우님 flow

## 1. 처음에 동우님이 장희레포에 깃 클론을 합니다.

<br />

## 2. 동우님이 브런치를 각각 dev와 local을 만듭니다.

<br />

## 3. 브런치 만들기

### dev 브런치 만들기

```
git switch -c dev
git push origin dev
```

<br />

### local 브런치 만들기

```
git switch -c local
git push origin local
```

<br />

## 4. local에서 작업하기

- 로컬에서 동우님 프로젝트 진행하기

<br />

## 5. local작업 깃 푸쉬하기 (본인 레포에)

```
git branch (로컬인지 아닌지 확인)
git switch local 

git status
git add .
git commit -m "메세지"
git push origin local
```

<br />

## 6. local이 확실하면 dev브런치에 병합니다.

```
git switch dev
git merge local
git push origin dev
```

<br />

## 7. 동우님레포에서 PR 요청을 합니다.

<br />

## 8. 장희님의 작업이 끝나서 장희님 작업을 가져오려고 합니다.

```
git remote -v
git remote add {작명} {장희님의레포주소}
git remote -v
git pull {작명} dev
git push origin dev
```

---

# 장희님 flow

## 1. 레포를 만들어서 깃에 올립니다. (콜라보레이터 초대 하기!)

<br />

## 2. 브런치 만들기

### dev 브런치 만들기

```
git switch -c dev
git push origin dev
```

<br />

### local 브런치 만들기

```
git switch -c local
git push origin local
```

<br />

## 3. local에서 작업하기

- 로컬에서 장희님 프로젝트 진행하기

<br />

## 4. local작업 깃 푸쉬하기 (본인 레포에)

```
git branch (로컬인지 아닌지 확인)
git switch local 

git status
git add .
git commit -m "메세지"
git push origin local
```

<br />

## 5. local이 확실하면 dev브런치에 병합니다.

```
git switch dev
git merge local
git push origin dev
```

<br />

## 6. 동우님의 PR요청 받고 merge까지 하기

<br />

## 7. 동우님이 작업하신 프로젝트 파일 받아오기

```
git remote -v
git pull origin dev
git push origin dev
```

<br /> 

## 8. dev에서 작업한 내용을 main에다가 옮기기

위에 했던 local에서 dev로 merge한거랑 비슷하게 하면 됩니다.