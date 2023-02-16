# IT 💻📚

<h3>Network</h3>
스위치 : 네트워크 단위들을 연결하는 통신 장비. 처리 가능한 패킷의 숫자가 큼. </br>
 - L1 : 더미허브. 랜선이 꽂힌 모든 포트에 동일한 정보 전달. (OSI 물리계층) </br>
 - L2 : 스위칭 허브. 각 포트 별 bandwidth 부여. 디바이스의 mac주소를 알고 있음. </br>
 - L3 : 라우터. L2에서 TCP/IP를 사용. </br>
 - L4 : 로드밸런싱. 네트워크 패킷을 지정해둔 포트들로 분산하여 배분. 서비스를 분산하기 때문에 한 쪽의 이슈에 대응 가능. </br>
 - L7 : 웹방화벽, 보안 스위치. 패킷을 분석하여 데이터 확인 가능. </br>

<h4>OSI 7계층</h4>
 - L1 : 물리계층. 전기적, 기계적, 기능적인 특성을 이용한 통신. </br>
 - L2 : 데이터링크계층. 물리계층을 통해 송수신되는 데이터의 오류와 흐름을 관리하여 전달하는 역할. => mac 주소로 통신. </br>
 - L3 : 네트워크계층. 데이터를 목적지까지 가장 안전하고 빠르게 전달하는 기능(라우팅, 경로 설정) => IP 주소로 통신. </br>
 - L4 : 전송계층. TCP 프로토콜 이용. 양 끝단의 사용자들이 신뢰성 있는 데이터를 주고 받을 수 있도록 하여 상위 계층들이 데이터 전달의 유효성이나 효율성을 생각하지 않도록 해줌. 전송에 실패한 패킷들은 재 전송. => 패킷 생성 및 전송. </br>
  (TCP : 신뢰성. 연결지향적 / UDP : 비연결성, 실시간 응용 및 멀티태스킹, 헤더 단순) </br>
 - L5 : 세션계층. 데이터가 통신하기 위한 논리적인 연결. => TCP/IP 세션을 만들고 없애는 역할. 사용자 동기화, 오류 복구. 세션 확립/유지/중단 </br>
 - L6 : 표현계층. 데이터 표현이 상이한 응용 프로세스의 독립성 제공 및 암호화. => 코드 간의 번역, 데이터 형식의 구분자. 사용자의 명령어 완성 및 결과 표현. 포장/압축/암호화 </br>
 - L7 : 응용계층. 최종 목적지. 응용 서비스 수행. => UI, 사용자의 입출력 </br></br>
