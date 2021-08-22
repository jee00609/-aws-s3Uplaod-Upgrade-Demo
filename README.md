# aws-s3Uplaod-Upgrade-Demo

## 개요

![시작 화면](https://user-images.githubusercontent.com/31675804/130340919-f3e86d6a-31db-4661-87c6-aff67790618b.PNG)

브라우저에서 이미지와 오디오를 선택하여 AWS S3 버킷에 이미지를 업로드하는 프로젝트

[이전 이미지만을 업로드하는 프로젝트](https://github.com/jee00609/aws-s3Uplaod-Demo) 에서 기능을 추가하여 만들었다.

## IDE / Dependency

IDE : STS

Dependency : Maven

## 사용법

1. stc/main/resources 에 application.properties 변경

```properties
spring.mvc.view.prefix=/WEB-INF/VIEWS/
spring.mvc.view.suffix=.jsp

server.port=8080

spring.servlet.multipart.max-file-size=10485760
app.aws.iam.accesskey=Access Key
app.aws.iam.secretkey=Secret Key
app.aws.s3.clientregion=Region
app.aws.s3.bucketnameImage=Bucket Name that saves image file
app.aws.s3.bucketnameAudio=Bucket Name that saves audio file
```
참고로 10485760 는 10MB 를 의미한다.

2. 실행한다 (Run as Spring boot App)

## 참고
[참고 프로젝트](https://github.com/nadunc/AWS-S3-image-uploader-with-java-spring-boot)

## 참고 프로젝트와의 차이점

   * 이미지 사이즈
      * 5MB -> 10MB
   * WEB/INF 사용
      * HTML -> JSP
   * 오디오 파일 업로드 기능 
