# 💡 수강생 관리 프로그램

> 📘 **패스트캠퍼스 | 9개 도메인 프로젝트로 끝내는 백엔드 웹 개발 (Java/Spring) 초격차 패키지 Online**  
> 🧩 **Ch 02. 객체 지향 설계 실습 - 수강생 관리 프로그램 과제 실습**

---

## 📝 프로그래밍 요구사항

- 아래 유즈케이스를 기반으로 설계 후, `domain`, `application` 패키지 내부만 수정하여 객체지향적으로 구현합니다.
- **Java 코드 컨벤션은 [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)을 따릅니다.**
    - 👉 [IntelliJ에 적용하는 방법](https://www.notion.so/ea91a00678014af68125209bb0caf50c?pvs=21)
- 함수는 **하나의 일만 수행**하도록 작성합니다.
- 참고 자료:
    - 🔹 [Value Object](https://tecoble.techcourse.co.kr/post/2020-06-11-value-object/)
    - 🔹 [1급 컬렉션](https://f-lab.kr/insight/understanding-and-applying-first-class-collections)
    - 🔹 [객체지향 생활체조](https://jamie95.tistory.com/99)

---

## ✅ 유즈케이스 - 과외 수강생 관리 프로그램 기능

1. **요일별 수업 정보 조회**
    - `MONDAY`, `TUESDAY` 등 요일을 입력받아 해당 요일의 수업 목록을 출력
    - 단, 학생이 *비활성화 상태*일 경우 해당 학생의 수업은 출력되지 않음

2. **학생 상태 변경 기능**
    - *활성 상태* → 일별 수업에 포함됨
    - *비활성 상태* → 일별 수업에서 제외됨
    - 동일한 상태로는 변경할 수 없음 (예: 활성 → 활성 ❌)

3. **수강료 변경 기능**
    - 특정 학생의 수강료를 변경하면 **해당 학생의 모든 수업**에 반영됨
