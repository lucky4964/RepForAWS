# AWS Day1

MAZON AWS사용하여 VPC구성하기
----------------------------
1. Keypair 생성
2. VPC구성, Subnet 구성
  - Public Subnet
  - Private Subnet
  - Available Zone (가용 영역)
  - NAT Subnet
  - Internet Gateway
3. RDS
  - Database를 나누는 이유
4. Load Balance
5. AutoScailing


구성도
![alt text]()


### Keypair 생성



### VPC, Subnet 구성
console -> VPC 검색 -> Dashboad탭 -> VPC Wizard -> VPC with Public and Private Subnets
'''
  * [IPv4 CIDR 블록:*] : 10.0.0.0/16 -> subnet이 포함될 IP블록
  * [VPC 이름] : My Lab VPC
  * [퍼블릭 서브넷의 IPv4 CIDR:*] : 10.0.1.0/24 -> Public subnet1 IP
  * [가용 영역:*] : ap-northeast-2a
  * [퍼블릭 서브넷 이름:] : Public_Subnet1
  * [프라이빗 서브넷의 IPv4 CIDR:*] : 10.0.3.0/24 -> Private subnet1 IP
  * [가용 영역:*] : ap-northeast-2a
  * [프라이빗 서브넷 이름:] : Private_Subnet3
'''
같은 가용역역을 공유하므로써 위와 같이 하나의 AZ 에 묶였다.
Use a NAT instance instead를 눌러 Public Subnet1을 NAT instance로 사용한다.
Keypair는 이전에 만든 Keypair 사용



위와 마찬가지로 Public subnet2, Public subnet5, Private subnet4, Private subnet6를 생성하여 각각의 AZ에 묶는다.

#### Public Subnet
#### Private Subnet
#### Available Zone
#### NAT Subnet
#### Internet Gateway(IGW)

### RDS 구성

### Load Balance

### AutoScailing
