# 쿵짝 Kungjjak - 박자 연습기

박자를 고르고 시작을 누른 뒤 **짝 소리에 맞춰 패드를 누르면**, 맞았는지 **몇 ms 빠르고 늦었는지** 바로 알려 주는 웹 도구입니다.
설치도 가입도 없이 주소만 열면 됩니다. 휴대폰에서 쓰기 좋게 만들었습니다.

## 👉 바로 쓰기

**https://henmoogi.github.io/kungjjak/**

1. 박자를 고릅니다: 2/4(행진곡), 3/4(왈츠), 4/4(가요·팝), 6/8, 12/8.
2. **시작**을 누르면 쿵(파랑)·짝(주황)·츠(회색) 칸에 차례로 불이 들어옵니다. 쿵에는 발을 구르고, 짝에 패드를 누릅니다.
3. 누를 때마다 '정확해요'(80ms 안), '조금 빨라요 ○ms', '조금 늦어요 ○ms'가 나옵니다.
4. 익숙해지면 빠르기를 올리거나, '짝 소리 빼고 내가 채우기'를 켜서 짝 소리 없이 내 박수로 채워 봅니다.

## 기능

- 박자마다 세는 법과 그 박자로 된 곡 예
- 빠르기 40~140 BPM, 마디 첫 박 종소리, 하이햇(츠) 소리 켜고 끄기
- 키보드 스페이스로도 누를 수 있음
- 고른 박자·빠르기·하이햇 설정은 이 기기에만 저장

## 서버로 보내는 것이 없습니다

- 페이지는 HTML 파일 하나(`index.html`)입니다. 소리는 브라우저가 바로 만들고(Web Audio) 마이크는 쓰지 않습니다. 누른 기록은 화면에만 보입니다.
- 외부에서 불러오는 것은 글꼴(Google Fonts)뿐입니다.

## 한계

- 블루투스 이어폰은 소리가 늦게 도착해서 '늦어요'가 많이 나올 수 있습니다. 휴대폰 스피커로 쓰세요.
- 아이폰은 무음 모드면 소리가 나지 않을 수 있습니다.
- 브라우저가 알려 주는 소리 지연(outputLatency·baseLatency)만큼 빼고 판정합니다. 그 값을 주지 않는 브라우저나 화면 터치가 늦게 잡히는 기기에서는 판정이 '늦어요' 쪽으로 조금 밀릴 수 있습니다.
- '정확해요'의 기준(짝 소리 앞뒤 80ms)은 이 도구가 정한 값입니다.
- 곡 예는 대표적인 악보 표기를 따랐습니다. 6/8과 12/8은 같은 곡도 악보마다 다르게 적기도 합니다.
- 개인이 만든 연습 도구입니다.

---

## English

**Kungjjak** is a beat practice tool: pick a time signature (2/4, 3/4, 4/4, 6/8, 12/8), press start, and tap the pad on the snare ("jjak"). It tells you right away whether you were on time or how many milliseconds early or late.
No install, no sign-up: **https://henmoogi.github.io/kungjjak/** (Korean interface). Sound is generated in the browser; nothing is sent to a server.

## 라이선스 License

[MIT](LICENSE). 무보증입니다. No warranty.
