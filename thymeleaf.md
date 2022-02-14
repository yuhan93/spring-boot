thymeleaf 템플릿 엔진

\- 동작 환경

![image](https://user-images.githubusercontent.com/56163121/153870565-7126b868-67a8-4353-9d8b-42c8827751ce.png)

컨트롤러에서 리턴 값으로 문자를 반환하면 뷰 리졸버( viewResolver ) 가 화면을 찾아서 리턴한다.

\- 스프링 부트 템플릿엔진 기본 viewName 매핑

\- resources : tmplates/ + { ViewName } + .html

```java
@Controller
public class HelloController {

    @GetMapping("hello")
    public String hello(Model model){
        model.addAttribute("data", "hello!!");
        return "hello";
    }

}
```

---

![image](https://user-images.githubusercontent.com/56163121/153870518-fac3d051-b196-4be6-bf6f-7d873f4dd3b3.png)

---
![캡처](https://user-images.githubusercontent.com/56163121/153870420-349e393f-f524-42ef-92d7-8a82cf64d190.PNG)
