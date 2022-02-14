thymeleaf 템플릿 엔진

\- 동작 환경

[##_Image|kage@bEuanh/btrtlaN0p3h/sPwXOwDnfxS7wmBLq7BGJK/img.png|CDM|1.3|{"originWidth":617,"originHeight":314,"style":"alignCenter"}_##]

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

[##_Image|kage@z86x6/btrtlURAh24/N2oCgq3yg8ZL8uV6zKzFV0/img.png|CDM|1.3|{"originWidth":725,"originHeight":338,"style":"alignLeft"}_##]

---

[##_Image|kage@b2terV/btrtlorRdBJ/WKKPDFA46RYK49ZFvFmTQk/img.png|CDM|1.3|{"originWidth":313,"originHeight":124,"style":"alignCenter"}_##]