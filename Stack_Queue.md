# 스택 & 큐
- 임의의 위치에 항목 삽입/삭제 가능한 자유로운 리스트와 달리 스택&큐는 항목의 접근이 맨 앞이나 맨 뒤로 제한 되는 선형 구조
- 관련 메소드
  push(item): 삽입 연산
  pop(): 삭제 연산
  len(): 리스트 항목 수 
  isEmpty(): 스택 혹은 큐가 비어있으면 True 아니면 False 반환
  peek(): 스택 혹은 큐 맨 위/앞에 있는 항목을 삭제하지않고 반환 
  size(): 항목들의 개수 반환
  clear(): 공백상태로 만듬

  ![](https://images.velog.io/images/felizcarol/post/bb9c93a4-5091-4765-9a76-c1e7ee0f3e3d/image.png)


- 스택 (Stack)
  - 후입 선출 (LIFO: Last-In First Out)
  - 응용: 편집 되돌리기(undo), 웹브라우저 이전 페이지 이동, 괄호 검사 알고리즘, 계산기 프로그램 (전위, 중위, 후위), 깊이우선탐색, 미로탐색 등
  
```python
bts = []
# 리스트에 push 
bts.append('V')
bts.append('Jin')
bts.append('RM')
bts.append('Suga')
# pop 사용하여 'Suga' 꺼내기
last_member = bts.pop()
print(last_member)
# 남은 멤버
print(bts)
```
- 큐 (Queue)
   - 큐의 첫 원소(front), 끝 원소 (rear)
   - 선입 선출 (FIFO: First-In First Out)
   - enqueue(): 삽입 연산, dequeue(): 삭제 연산
   - 응용: 프린터 인쇄 작업, 동영상 버퍼링, 너비우선탐색 등

```python 
blackpink = []
blackpink.append('Jennie')
blackpink.append('Lisa')
blackpink.append('Jisoo')
blackpink.append('Rosé')
first_member = blackpink.pop(0)
print(first_member) # ['Jennie'] 
first_member = blackpink.pop(0)
print(first_member) # ['Lisa'] 
print(blackpink) # 남은 멤버['Jisoo', 'Rosé']
