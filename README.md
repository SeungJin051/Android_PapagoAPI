# 오픈API 활용하기 PapagoAPI

[![Video Label](http://img.youtube.com/vi/fHB_O5D60lo/0.jpg)](https://youtu.be/fHB_O5D60lo)

<hr>

![21952_32934_4438](https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/99f06832-2321-498e-aa57-8dc9d9719017)

  * API
    * 운영체제나 시스템, 애플리케이션, 라이브러리 등을 활용해 응용 프로그램을 작성할 수 있게 하는 다양한 인터페이스를 의미합니다. 

  * 오픈API
    * API 중에서 플랫폼의 기능 또는 콘텐츠를 외부에서 웹 프로토콜(HTTP)로 호출해 사용할 수 있게 개방(open)한 API를 의미합니다. 네이버 개발자센터에서 제공하고 있는 지도, 검색을 비롯 기계 번역, 캡차, 단축 URL 등 대부분 API는 HTTP로 호출할 수 있는 오픈 API에 해당합니다.

<hr>

## 네이버 Papago API
  [네이버 개발자 센터](https://developers.naver.com/main/)
  1. 풍부한 언어 처리 경험 : 인공신경망 번역 엔진으로 문장 전체를 더욱 정확하고 문장 맥락에 맞는 번역을할 수 있습니다.
  2. 번역 지원 언어 : 13개 언어를 지원합니다. (처리한도 : 10,000글자/일)
  3. 손쉬운 사용 : 웹 기반의 콘솔을 통해 쉽고 편리한 사용이 가능합니다. RESTful 형태로 지원되는 API를 통해 고객의 서비스에 번역 기능을 간단하게 적용할 수 있습니다.
  4. 신청 방법 : 네이버 개발자 센터에서 API KEY를 신청합니다.

<hr>
 
## Papago 번역 언어 코드 및 지원 언어
<img width="753" alt="스크린샷 2023-05-20 오후 11 18 17" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/9a1580ce-d663-4d5a-8d13-f590766632f4">

<hr>

# API 키 생성 

<img width="500" alt="seukeurinsyas-2023-05-20-ojeon-11 51 53" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/e26dfea4-49bc-485d-8e09-06934f8bdb37">

 ## 네이버 개발자 센터 접속 - 네이버 개발자 센터에서 Papago 클릭.
 
 <img width="500" alt="seukeurinsyas-2023-05-20-ojeon-11 52 03" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/1879886a-c617-4af6-a824-803b943e7ede">
 
  ## PaPago 번역 - 파파고 번역 오픈 API 이용신청

<img width="500" alt="seukeurinsyas-2023-05-20-ojeon-11 53 24" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/5f5674bf-31ce-42ff-93aa-9f2f9eb0a032">

  ## 안드로이드 스튜디오 Create Project - 애플리케이션 등록을 위해 프로젝트 패키지 이름이 필요하기에 프로젝트를 만들어준다.
  
<img width="500" alt="seukeurinsyas-2023-05-20-ojeon-11 53 39" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/bf684c9c-6432-43e1-b129-c957e891bd22">

  ## 애플리케이션 등록 (API 이용신청) - 개발자의 목적에 따라 설정을 해준다.
  
<img width="500" alt="seukeurinsyas-2023-05-20-ojeon-11 54 03" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/49e238db-46ee-40fc-b0cf-6b35f20bc5f0">

  ## 애플리케이션 등록 완료! - 본인의 Client ID, Client Secret를 확인한다.
  
  <img width="500" alt="seukeurinsyas-2023-05-20-ohu-1 10 11" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/37848714-c1bd-4764-8494-36a4fd4671c0">

  ## 개발자 콘솔 - 본인이 신청한 애플리케이션의 목록을 볼 수 있다.
  
<hr>

# API 가이드
 1. 이용 비용 - 무료로 제공되는 서비스로, 일일 이용량 제한이 존재합니다.
 2. 보안 유지 - API의 KEY 데이터 및 개인정보 보안 유지를 위해 주의합니다.

<hr>
 
# API 흐름
 <img width="500" alt="스크린샷 2023-05-20 오후 11 25 35" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/38d7e154-780a-4e6d-8676-f4a6c358989d">
 
<hr>

# API 사용 방법
 * API 게이트웨이
   * 네이버 오픈API는 대부분 https://openapi.naver.com/(request URL) 게이트웨이서버를 통해 API를 호출합니다. API 게이트웨이는 오픈 API 호출이 들어오면 API 호출이 정확한지, 인증된 사용자의 호출인지, 호출 허용량이 맞는지 등을 확인한 다음 실제 각 API 서버를 호출한 결괏값을 반환합니다.
 * API 키 또는 키
   * API 키(클라이언트 아이디와 클라이언트 시크릿)는 인증된 사용자임을 입증하는 고유한 텍스트 문자열입니다.
 
<hr>

# 참고 사항
 <img width="896" alt="seukeurinsyas-2023-05-20-ohu-2 19 48" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/32a0e767-7fa2-447d-b239-522543b5cd1b">
 
<hr>

# Documents Papago 샘플 코드
 ``` java
 import java.io.BufferedReader;
import java.io.DataOutputStream;
import java.io.InputStreamReader;
import java.net.HttpURLConnection;
import java.net.URL;
import java.net.URLEncoder;
import java.util.Map;

// 네이버 기계번역 (Papago SMT) API 예제
public class ApiExamTranslateNmt {

    public static void main(String[] args) {
        String clientId = "YOUR_CLIENT_ID";//애플리케이션 클라이언트 아이디값";
        String clientSecret = "YOUR_CLIENT_SECRET";//애플리케이션 클라이언트 시크릿값";

        String apiURL = "https://openapi.naver.com/v1/papago/n2mt";
        String text;
        try {
            text = URLEncoder.encode("안녕하세요. 오늘 기분은 어떻습니까?", "UTF-8");
        } catch (UnsupportedEncodingException e) {
            throw new RuntimeException("인코딩 실패", e);
        }

        Map<String, String> requestHeaders = new HashMap<>();
        requestHeaders.put("X-Naver-Client-Id", clientId);
        requestHeaders.put("X-Naver-Client-Secret", clientSecret);

        String responseBody = post(apiURL, requestHeaders, text);

        System.out.println(responseBody);
    }

    private static String post(String apiUrl, Map<String, String> requestHeaders, String text){
        HttpURLConnection con = connect(apiUrl);
        String postParams = "source=ko&target=en&text=" + text; //원본언어: 한국어 (ko) -> 목적언어: 영어 (en)
        try {
            con.setRequestMethod("POST");
            for(Map.Entry<String, String> header :requestHeaders.entrySet()) {
                con.setRequestProperty(header.getKey(), header.getValue());
            }

            con.setDoOutput(true);
            try (DataOutputStream wr = new DataOutputStream(con.getOutputStream())) {
                wr.write(postParams.getBytes());
                wr.flush();
            }

            int responseCode = con.getResponseCode();
            if (responseCode == HttpURLConnection.HTTP_OK) { // 정상 응답
                return readBody(con.getInputStream());
            } else {  // 에러 응답
                return readBody(con.getErrorStream());
            }
        } catch (IOException e) {
            throw new RuntimeException("API 요청과 응답 실패", e);
        } finally {
            con.disconnect();
        }
    }

    private static HttpURLConnection connect(String apiUrl){
        try {
            URL url = new URL(apiUrl);
            return (HttpURLConnection)url.openConnection();
        } catch (MalformedURLException e) {
            throw new RuntimeException("API URL이 잘못되었습니다. : " + apiUrl, e);
        } catch (IOException e) {
            throw new RuntimeException("연결이 실패했습니다. : " + apiUrl, e);
        }
    }

    private static String readBody(InputStream body){
        InputStreamReader streamReader = new InputStreamReader(body);

        try (BufferedReader lineReader = new BufferedReader(streamReader)) {
            StringBuilder responseBody = new StringBuilder();

            String line;
            while ((line = lineReader.readLine()) != null) {
                responseBody.append(line);
            }

            return responseBody.toString();
        } catch (IOException e) {
            throw new RuntimeException("API 응답을 읽는데 실패했습니다.", e);
        }
    }
}
 ```
<hr>

# API 활용 앱 With ChatGPT

 ## 프로젝트 Manifest 퍼미션 추가
  ``` java
    <!--  인터넷 통신을 위한 퍼미션  -->
    <uses-permission android:name="android.permission.INTERNET"/>
  ```
  
 ## 프로젝트 API KEY 설정 
 ``` java
            String clientId = "네이버 API 클라이언트 아이디";                      
            String clientSecret = "네이버 API 클라이언트 시크릿";                        
            try {
                String text = URLEncoder.encode(et_target.getText().toString(), "UTF-8");  // 번역할 문장

                String apiURL = "https://openapi.naver.com/v1/papago/n2mt";
                URL url = new URL(apiURL);
                HttpURLConnection con = (HttpURLConnection) url.openConnection();
                con.setRequestMethod("POST");
                // 네이버 클라이언트 아이디 설정
                con.setRequestProperty("X-Naver-Client-Id", clientId);
                // 네이버 클라이언트 시크릿 설정
                con.setRequestProperty("X-Naver-Client-Secret", clientSecret);
                // 번역 소스 언어는 한국어(ko), 목표 언어는 영어(en), 번역할 텍스트는 변수 text에 저장된 값
                String postParams = "source=ko&target=en&text=" + text;
 ```
 
 ## 프로젝트 API 요청 성공
 ``` java
                 // HTTP 요청이 성공
                if (responseCode == 200) {
                    // 번역 결과를 문자열 형태로 저장
                    String result = response.toString();
                    // response에서 "translatedText" 다음에 오는 값만 추출하여 번역된 텍스트를 얻음
                    // 추출한 텍스트는 translationResult 변수에 저장
                    번역결과 = result.split("\"translatedText\":\"")[1].split("\"")[0];
                } else {
                    번역결과 = "번역 실패";
                }
 ```
 
 <img width="500" alt="스크린샷 2023-05-20 오후 12 34 17" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/29a90298-bffd-4cf8-8d4f-0645a92b0644">

 ## JSON 데이터 교환 형식
  * 네이버에 번역하고 싶은 단어나 문장을 보내주면   해당 문장을 번역한 결과값을 JSON으로 반환.
    * translatedText.value만 가져와 result에 넣는다.

## 응답
<img width="700" alt="seukeurinsyas-2023-05-20-ohu-2 14 38" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/474d6398-59f0-4acb-a106-3864b612cdc1">

## 오류 코드
<img width="700" alt="seukeurinsyas-2023-05-20-ohu-2 15 38" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/014bbe64-5d1d-43f6-b3e3-fe04c4167583">

## 네이버 Papago API를 활용한 번역 앱
<img width="400" alt="스크린샷 2023-05-20 오후 11 36 16" src="https://github.com/SeungJin051/Android_PapagoAPI/assets/83889135/ce533c9b-0a37-4545-b134-be5f53956ef5">

 
