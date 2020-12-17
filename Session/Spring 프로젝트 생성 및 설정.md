## Spring 프로젝트 생성 및 기본 설정

1. XML 파일 보기 설정 - 상단 메뉴바에서 Window -> Preferences

   ![xml파일 설정1](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\xml파일 설정_1.png)

   

2. XML 파일 보기 설정2 - Gerneral -> Editors -> File Associations에서 *.xml파일 선택 후 하단에서 XML Editor를 Default로 설정한다. 

   ![xml파일 설정2](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\xml파일 설정_2.png)

   

3. 프로젝트 생성 - File -> New -> Spring Legacy Project 클릭 또는 프로젝트 탐색기에서 오른쪽 클릭 후 New -> Spring Legacy Project

   ![](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\프로젝트 생성_1.png)

   

4. 프로젝트 생성 - 이후 생성할 프로젝트에 대한 설정을 합니다. 기본적인 Project name을 설정하고, 생성할 프로젝트의 템플릿을 설정합니다. 여기선 API Server를 위한 MVC 패턴을 틀로 주는 Spring MVC Project로 선택하고 Next를 클릭합니다.

   ![](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\프로젝트 생성_2.png)

   

5. 프로젝트 생성 - 생성할 프로젝트에 적용할 패키지 레벨을 적어줍니다. 기본적으로 Spring의 프로젝트는 3 Level이상으로 아래 처럼 작성하여야합니다. 

   ![](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\프로젝트 생성_3.png)

   

6. 프로젝트 생성 - 마지막으로 프로젝트를 구성하는데 필요한 라이브러리들을 다운로드받으면 프로젝트에 표시되던 에러가 사라지게 됩니다.

   ![](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\프로젝트 생성_4.png)

   

7. tomcat 연동 - 왼쪽 하단의 Servers 탭에서 오른쪽 클릭 후 -> New -> Server를 통해 Server 추가를 진행합니다.

   ![tomcat 연동_1](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 연동_1.png)

   

8. tomcat 연동 - Apache -> 추가할 Tomcat 버전 선택 -> Add Configure runtime environments(실행할 tomcat을 설정하는것)

   ![tomcat 연동_2](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 연동_2.png)

   

9. tomcat 연동 - 이후 나온 Preferences 창에서 -> Server -> Runtime Environments -> Add 클릭을 통해 새로운 Server 실행환경을 추가합니다.

   Add 클릭시 나오는 New Server Runtime Environment 창에서 추가할 Name(서버설정 이름)과 Tomcat installation directory(설치한 Tomcat의 폴더 위치), JRE(Tomcat을 실행할 때 이용할 jdk,jre를 설정)들을 설정합니다.

   이후 Finish 클릭

   ![tomcat 연동_3](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 연동_3.png)

   

10. tomcat 연동 - 추가한 서버설정을 클릭하고 Apply and Close 클릭

    ![tomcat 연동_4](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 연동_4.png)

    

11. tomcat 연동 - 다시 New Server 창으로 돌아와서 추가할 Server Name과 방금 설정한 Server runtime environment(서버 실행환경)을 지정하고 -> Next 클릭

    ![tomcat 연동_5](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 연동_5.png)

    

12. tomcat 연동 - 추가하는 Tomcat Server와 연동 시킬 프로젝트를 선택합니다.

    이동 방법은 좌측의 가능한 프로젝트들 중 원하는 프로젝트를 더블 클릭 또는 선택 후 Add 버튼을 통해 옮길 수 있습니다.

    제거 역시 우측에서 더블 클릭 또는 선택 후 Remove 버튼 클릭을 통해 제거 할 수 있습니다.

    선택 완료 후 Finish 버튼 클릭

    ![tomcat 연동_6](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 연동_6.png)

    

13. tomcat 설정 확인 - Spring 좌측 하단의 추가된 Server를 더블클릭 합니다.

    ![tomcat 설정_1](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 설정_1.png)

    

14. tomcat 설정 확인 - 처음으로 Overview탭의 설정내용이 보이며, 이 곳에서 서버실행환경 또는 실행하는 포트번호 설정 등을 할 수 있습니다.

    ![tomcat 설정_2](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 설정_2.png)

    

15. tomcat 설정 확인 - 마지막으로 하단의 Modules 탭에서는 현재 서버가 실행되는 기본 url을 확인할 수 있습니다.

    아래 Server의 경우는 http://localhost:8080/mvc 가 기본 url입니다.

    ![tomcat 설정_3](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 설정_3.png)

    

16. tomcat 실행 및 접속 - 좌측 하단에서 실행할 Server를 선택하고 start 버튼을 클릭합니다.

    상단의 붉은색 박스는 각각 순서대로 디버깅 모드로 실행, 서버 실행, 서버 정지 버튼입니다. 

    서버 실행 후 http://localhost:8080/mvc 로 접속할 경우 아래와 같은 화면을 확인할 수 있습니다.

    ![tomcat 실행](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\tomcat 실행.png)

    

17. 접속 후 화면

    ![기본화면](C:\Users\tpdls\Desktop\HSY\Spring프로젝트 설정 및 만들기\기본화면.png)

    

