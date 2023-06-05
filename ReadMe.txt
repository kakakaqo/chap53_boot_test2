[스프링 부트 단위테스트]

 
 - 컨트롤러 단위테스트
 

1. 의존성
 - 스프링 부트 버전을 2.7.12 버전으로 변경
  이걸 변경하게 되면 매퍼XML의 vo Alias 문제 사라짐.
 - 그래도 안되면 validation에서 Mapper XML 검증 해제할것.

	<dependencies>
 		<!--추가-->
		<!-- JUnit Jupiter API -->
	    <dependency>
	        <groupId>org.junit.jupiter</groupId>
	        <artifactId>junit-jupiter-api</artifactId>
	        <scope>test</scope>
	    </dependency>
	    
	    <!-- JUnit Jupiter Engine -->
	    <dependency>
	        <groupId>org.junit.jupiter</groupId>
	        <artifactId>junit-jupiter-engine</artifactId>
	        <scope>test</scope>
	    </dependency>
	    
	    <!-- Mockito Core -->
	    <dependency>
	        <groupId>org.mockito</groupId>
	        <artifactId>mockito-core</artifactId>
	        <scope>test</scope>
	    </dependency>
	    
	    <!-- Mockito JUnit Jupiter -->
	    <dependency>
	        <groupId>org.mockito</groupId>
	        <artifactId>mockito-junit-jupiter</artifactId>
	        <scope>test</scope>
	    </dependency>
	    
[주의]

1. 매퍼XML에서 vo를 풀 경로가 아니고 이름만 사용할 경우 빨간 밑줄 
 - Window > preference > validation > MyBatis Mapper Validator 체크 해제
 	    
