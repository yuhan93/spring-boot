API
---
@ResponseBody 객체 변환

![image](https://user-images.githubusercontent.com/56163121/157430565-a29b1b07-d676-4abf-b9cd-011eee2cff15.png)
-   @ResponseBody 를 사용하면 뷰 리졸버 ( viewResolver ) 를 사용하지 않는다.
-   대신에 HTTP의 BODY에 문자 내용을 직접 반환한다. ( HTML BODY TAG 를 말하는 것이 아니다 )
---

@ResponseBody 객체 반환

![image](https://user-images.githubusercontent.com/56163121/157430632-5094925f-12cd-4476-b269-7d3260bd6fd5.png)
-   @ResponseBody를 사용하고, 객체를 반환하면 객체가 JSON으로 변환이 된다.

---
@ResponseBody 사용 원리

![image](https://user-images.githubusercontent.com/56163121/157430709-50acad58-ad5e-4ca9-a0e5-8f2d5e33860b.png)
-   @ResponseBody를 사용
-   HTTP의 BODY에 문자 내용을 직접 반환한다
-   viewResolver 대신에 HttpMessageConverter가 동작한다.
-   기본 문자 처리 : StringHttpMessageConverter 
-   기본 객체 처리 : MappingJackson2HttpMessageConverter
-   byte 처리 등등 기타 여러 HttpMessageConverter 가 기본으로 등록 되어 있다.
