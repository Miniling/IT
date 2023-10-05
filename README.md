# IT 💻📚

<h2>Network</h2>
스위치 : 네트워크 단위들을 연결하는 통신 장비. 처리 가능한 패킷의 숫자가 큼. </br>
 - L1 : 더미허브. 랜선이 꽂힌 모든 포트에 동일한 정보 전달. (OSI 물리계층) </br>
 - L2 : 스위칭 허브. 각 포트 별 bandwidth 부여. 디바이스의 mac주소를 알고 있음. mac주소를 활용하여 데이터를 전달하면 L2 장비. </br>
 - L3 : 라우터. L2에서 TCP/IP를 사용. IP주소를 활용하여 데이터를 전달하면 L3 장비. </br>
 - L4 : 로드밸런싱. 네트워크 패킷을 지정해둔 포트들로 분산하여 배분. 서비스를 분산하기 때문에 한 쪽의 이슈에 대응 가능. </br>
 - L7 : 웹방화벽, 보안 스위치. 패킷을 분석하여 데이터 확인 가능. </br>
</br>
 - Mesh Topology : 망형. 거미줄처럼 엮여있는 형태. 하나가 끊겨도 연결 유지. 대량 데이터의 이동에도 병목 현상 최소화. 대규모 백본 네트워크에서 주로 사용. 구조 복잡. 모든 노드가 전부 연결되어있으면 Full-Mesh, 부분만 연결되어있으면 Partial-Mesh.  </br>
 - Ring Topology : 원형. 1:1 매칭. </br>
 - Star Topology : 중앙 장치 주변에 위성 장치 존재. </br>
 - Tree Topology : Star Topology의 복수 형태. </br>
 - Bus Topology : 통신선 공유. 차량용에 가장 많이 사용. 사용되는 선 감소. </br>
</br>

MPLS : Multi-Protocol Label Switching. 데이터 패킷에 라벨을 붙여 스위칭하고 라우팅하는 기술. 대량의 트래픽을 고속으로 처리 가능. </br>
NAC : Network Access Control. 시스템 인증 및 네트워크 보안 기술. 네트워크에 액세스 하려는 장치 식별 및 보안 인증. </br>
OFD : Optical Fiber Distribution. 광분배함. </br>
</br>

CRC : 순환중복검사(Cyclic Redundancy Check). 송신한 데이터를 수신측에서 검사(= 데이터 무결성 검사). 데이터에 붙은 값을 지정된 crc 다항식으로 나누어 나머지가 0이면 정상, 0이 아니면 오류.

<h4>OSI 7계층</h4>
 - 1계층 : 물리계층. 전기적, 기계적, 기능적인 특성을 이용한 통신. </br>
 - 2계층 : 데이터링크계층. 물리계층을 통해 송수신되는 데이터의 오류와 흐름을 관리하여 전달하는 역할. => mac 주소로 통신. </br>
 - 3계층 : 네트워크계층. 데이터를 목적지까지 가장 안전하고 빠르게 전달하는 기능(라우팅, 경로 설정) => IP 주소로 통신. </br>
 - 4계층 : 전송계층. TCP 프로토콜 이용. 양 끝단의 사용자들이 신뢰성 있는 데이터를 주고 받을 수 있도록 하여 상위 계층들이 데이터 전달의 유효성이나 효율성을 생각하지 않도록 해줌. 전송에 실패한 패킷들은 재 전송. => 패킷 생성 및 전송. </br>
  (TCP : 신뢰성. 연결지향적 / UDP : 비연결성, 실시간 응용 및 멀티태스킹, 헤더 단순) </br>
 - 5계층 : 세션계층. 데이터가 통신하기 위한 논리적인 연결. => TCP/IP 세션을 만들고 없애는 역할. 사용자 동기화, 오류 복구. 세션 확립/유지/중단 </br>
 - 6계층 : 표현계층. 데이터 표현이 상이한 응용 프로세스의 독립성 제공 및 암호화. => 코드 간의 번역, 데이터 형식의 구분자. 사용자의 명령어 완성 및 결과 표현. 포장/압축/암호화 </br>
 - 7계층 : 응용계층. 최종 목적지. 응용 서비스 수행. => UI, 사용자의 입출력 </br></br>

<h4>IP/Domain</h4>
 - IP: Internet Protocol. 인터넷 통신규약. ex) 192.168.1.255 </br>
 - Domain: 인터넷 사이트 주소. ex) github.com </br>
   ex) https://www.example.com => Protocol(프로토콜)=https://, Sub Domain=www, Domain Name=example, Top-Level Domain=com, Root Domain= Sub Domain + Top-level Domain </br>
 - URL: Uniform Resource Locator. 인터넷에서 각종 리소스의 위치를 가리키는 문자열 </br>
   ex) http://www.example.com:80 => Scheme(스키마)=https, Domain Name(도메인)=www.example.com, Port(포트번호)=80 </br>
   http=80port, https=443port (https는 도메인 뒤에 포트번호 생략, http는 도메인 뒤에 포트번호 입력해야 각 포트별 웹으로 접속 가능) </br>

<h4>Library</h4>
라이브러리 : 소프트웨어 개발에서 자주 쓰고 기초적인 함수들을 중복 개발하는 것을 피하기 위해, 표준화된 함수 및 데이터 타입을 만들어서 모아둔 것.</br>
 - DLL(Dynamic Link Library): 동적 링크 라이브러리. 여러 프로그램에서 동시에 사용할 수 있는 코드와 데이터를 포함하는 라이브러리.</br>
</br>

<h4>차량용 통신 및 네트워크</h4>
내부 통신 </br>
: 각 제어기에 맞춘 통신 방식 (CAN, LIN, FlexRay, Ethernet, MOST) </br>
 - CAN : Controller Area Network. 호스트 없이 장치들 간 통신. 가장 많이 사용. BOSH에서 개발한 차량용 통신 방식. </br>
 - FlexRay : 제어 명령 + 진단 통신에 주로 사용. CAN/TTP보다 빠르고 안정적. </br>
 - LIN : Local Interconnect Network. 차량 내 컴포넌트 간 통신을 위한 직렬 통신. 센서 정보를 다른 제어기에 전달할 때 사용. CAN에 비해 저렴. </br>
</br>
: 차량 내 멀티미디어 정보 활용, 센서의 데이터량 증가(카메라, 라이더, 레이더, ...) </br>
 - Ethernet : 컴퓨터 네트워크 기술. 멀티미디어, ADAS 등 대량 정보 통신. </br>
</br>

외부 통신 </br>
(무선 통신. LTE, DSRC, Wi-Fi, Bluetooth, ...) </br>
: 차량 간 통신, 차량↔인프라 통신 </br>
 
 - 진단 통신 : 정비소 차량 진단 (CAN, Ethernet 방식 사용) </br>
 정보량 증가에 따라 Ethernet 통신 활용↑ </br>
  </br>
전기차 </br>
 충전기 연결 시, 자동차↔충전기 통신(PLC, Power Lince Communication. 전원 선을 이용한 통신) 배터리 정보 공유. </br>
 자율주행/커넥티드 카 => 내/외부 통신 사용. </br>
 </br>
 
<h4>CAN</h4>
물리 계층 </br>
  - 네트워크의 구성 </br>
  - 통신 선의 길이 </br>
  - 메인 선에서 제어기까지의 거리 </br>
  - Twisted wire를 이용한 통신 선 구성 </br>
  - 통신 속도 조절 가능 10kbps ~ 1000kbps(1Mbps) 최대 속도 = 선 길이 최대 40m. => 차량에는 일반적으로 500kbps, 1300m 사용 </br>
  - 통신 양 끝단에 종단 저항 설치. => 판사파 현상 제거하기 위함. </br>
  - 통신 선 2, 종단 저항 2 필요. </br>
  - Star, Ring, Bus Topology 모두 가능하나, 주로 Bus Topology 사용. </br>
   </br>
  동작 원리 </br>
   - Differential signal : 두 신호선에 발생하는 전압 차로 0, 1 구분. </br>
   - 외부의 진동, 전자기파에 의한 신호의 왜곡 발생 -> 전압 차이 유지 -> 1/0 판별 문제 없음. => CAN 통신이 매우 안전한 통신 방식인 이유. </br>
   - CAN_H ↔ CAN_L 두 통신선 전압 차이로 0/1 판별. (Recessive(1), Dominant(0) => 두 신호 충돌 시 0의 신호가 이김) </br>
   - Transceiver를 통해서 자동 개발. (발신자/수신자 합성어) CAN_H, CAN_L 신호 모두 생성. </br>
   - TTL 레벨 신호 -> CAN Differential 신호 생성. </br>
   - Transceiver를 이용해 통신 물리 계층 구현. </br>
 </br>
 데이터링크 계층 </br>
  SOF | Arbitration Field | Control Field | Data Field | CRC | ACK | End of Frame </br>
  - Data Frame : 정보를 담고 있는 그릇 </br>
  - SOF : Start of Frame. Single Dominant bit (시작. 프레임 포멧 정의) </br>
  - Arbitration Field (메시지 구분용 인덱스 넘버 지정) </br>
   - 11 bit Identifier </br>
   - 1 bit RTR(Remote Transmission Request): Dominant for data frames, recessive for remote frames </br>
  - Data Field : 센서 정보 </br>
  - CRC(Cyclic Redundancy Check) </br>
   - 15 bit CRC with generator polynomial X^15 + X^14 + X^10 + X^8 + X^7 + X^4 + X^3 + 1 </br>
   - 1 bit CRC delimiter: single(always) recessive bit </br>
  - ACK(Acknowledgement) </br>
   - 1 bit ACK slot: dominant overwriting </br>
   - 1 bit ACK delimiter: single(always) recessive bit </br>
  - End of Frame: 7 recessive bits (끝. 프레임 포멧 정의) </br>
   </br>

<h4>CAN 통신 데이터링크 계층</h4>
CRC : 수신한 데이터를 안전하게 받았는지를 수신 확인으로 데이터 안정성 보장 </br>
ACK: 수신 측에서 제대로 전달됐고, 정확하다를 판단하기 위해 알려줌. 정확한 데이터 수신 시 발신자에게 알림. </br>
CAN은 부가 정보를 이용하여 안정적인 데이터를 전달.  </br>
 </br>
데이터링크 계층 동작 원리 </br>
- Arbitration Field (중재) 필드 </br>
  : 메시지 구분용 ID 존재. 숫자로 표현. (ex. 엔진:0, 브레이크:1, ...) </br>
   메시지 간 우선순위 선정에도 사용. </br>
   각 제어기는 순차적으로 메시지를 보낼 필요가 있음 => 번호가 낮을 수록 높은 우선 순위 </br>
   각 제어기에서 동시에 메시지를 보내려고 했을 경우, 번호가 더 낮은 메시지를 먼저 전달(수행) 후에 다음 메시지 실행 </br>
   안전에 민감한 경우: 낮은 번호.  안전과 거리가 있는 경우: 높은 번호  => 메시지 우선 순위 결정 </br>
   데이터의 형태 + 메시지의 정보 </br>
 </br>

<h4>LIN 통신의 구조와 원리</h4>
LIN(Local Interconnect Network) </br>
: 서브 네트워크 방식=> 간단한 기능 제어에 사용. </br>
  single wire 방식. </br>
  최대 속도 20kbps => 저가/저속 통신으로 많이 사용됨. </br>
  5개 자동차 회사와 반도체 개발 회사가 개발 </br>
  => 국제 표준으로 정의. </br>
   간단한 기능의 ECU 제어용 로컬 네트워크 (센서, 액추에이터, 스위치) </br>
  노드 16개 이하. 메시지 64개 이하. </br>
  CAN 네트워크의 서브 네트워크로 사용. </br>
  한 제어기의 서브로 센서나 액추에이터에 사용 </br>
  Single Master/Multi Slave 구조 </br>
  : 명령을 내리는 Master, 명령을 수행하는 Slave. </br>
    Master <-> Slave LIN-Bus로 연결 (선 1개) </br>
   Time-triggered Schedule Communication </br>
    : 시간을 정해놓고 데이터 전달 </br>
    single-wire 방식에 적합 </br>
    Master의 스케줄에 따른 Slave 동작  </br>
 </br>
</br>

<h2>클라우드</h2>
클라우드(Cloud) : 네트워크 관리자들 사이에서 인터넷이 '구름처럼' 미지의 공간으로 가려져 있다고 표현하면서 시작됨. </br>
  - AWS : 클라우드 컴퓨팅은 인터넷을 통해 컴퓨팅 파워. 데이터베이스 저장 공간. 앱 및 기타 IT 자원을 클라우드 서비스 플랫폼에서 고객에게 제공하고 비용을 받는 것. </br>
  - 가트너 : 인터넷 기술을 활용해 많은 고객들에게 수준 높은 확장성을 가진 자원들을 서비스로 제공하는 컴퓨팅의 한 형태. </br>
  - IBM : 웹 기반의 응용 소프트웨어를 활용해 인터넷 가상공간에서 대용량 데이터베이스를 분산 처리하고, 컴퓨터나 휴대전화, PDA 등 다양한 단말기에서 데이터를 불러오거나 가공할 수 있게 만들어 주는 환경. </br>
</br>
  아마존은 2006ㅐ년에 아마존 웹 서비스에서 클라우드를 통해 저장 공간과 연산 자원을 제공하는 서비스인 S3와 EC2 개시. </br>
  => 세일 기간이 아니면 사용하지 않는 서버를 다른 기업에게 빌려주자는 취지에서 오늘날의 클라우드 탄생. </br>
</br>
  장점 : 접속의 편리함 - 사무실이 아닌 환경에서도 근무 가능, 서버상의 유연성 - 필요한 만큼의 컴퓨팅 자원 추가 가능, 서비스를 원하는 만큼만 사용하고 비용 부담. </br>
  단점 : 데이터를 외부에 보관하면서 생기는 불안감 - 데이터 유출 유려, 비용 효율성 - 서버 운영 비용이 많이 드는 기업은 비용 부담, 클라우드 의존도 - 다른 클라우드로 이전하는 호환성 문제(서비스 변경 불가) </br>
</br>
  On-Premise : 서버실. 서버에 직접 설치해서 운영하는 전통 방식. 보안 강력. 비용 과다. </br>
  Off-Premise : On-Premise의 가상화. </br>
</br>
  가상화는 물리적 인프라에 별도의 컴퓨팅 환경을 만드는 소프트웨어. </br>
  클라우드는 인터넷을 통해 고객이 요구하는 컴퓨팅 자원을 곧바로 제공하는 On-demand 방식의 서비스. </br>
</br>
  서버 가상화 -> 클라우드 </br>
</br>
  클라우드 서비스의 종류 </br>
  : IaaS, PaaS, SaaS, DaaS, BaaS, FaaS, DBaaS </br>
</br>
  - IaaS : 사용자가 관리할 수 있는 범위가 가장 넓은 클라우드 서비스. 컴퓨팅 자원 제공. 서버 운영체제, 미들웨어, 런타임, 데이터, 어플리케이션을 사용자가 직접 구성하고 관리 가능. (ex. Netflix) </br>
  - PaaS : IaaS 형태의 클라우드에 사용자가 원하는 서비스를 개발할 수 있도록 개발 환경을 미리 구축하여 제공하는 클라우드 서비스. 개발 서비스와 비즈니스에 집중 가능. 관리상 자유도는 낮음. </br>
  - SaaS : 사용자가 장치에 관계없이 어디에서나 SaaS 어플리케이션에 로그인할 수 있게 해주는 서비스. 사용자에게 큰 유연성 제공. 장치를 변경해도 다시 설치하거나 라이선스를 새로 구매할 필요x (ex. Google-Gmail 계정으로 구글 서비스 모두 이용 가능) </br>
  - DaaS : 재택 근무가 가능하도록 환경을 제공해주는 서비스. </br>
  - BaaS : 어플리케이션 개발에 필요한 서비스. </br>
