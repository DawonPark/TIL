# 인터넷은 어떻게 동작 하는가?

## 네트워크

![네트워크](https://mdn.mozillademos.org/files/8449/internet-schema-5.png)

- 단순하게 네트워크를 생각한다면 두개의 컴퓨터가 통신이 필요할 때, 우리는 다른 컴퓨터와 물리적으로 이더넷 케이블이나 무선 (WIFI, Bluetooth)으로 연결해야한다.
하지만 하나 하나 연결을 한다면 케이블의 수는 너무 많이 필요하다. 그렇기 때문에 각 집단을 연결할 라우터가 필요하고 이 구조로 무한히 확장이 가능하다.


![네트워크-모뎀](https://mdn.mozillademos.org/files/8451/internet-schema-6.png)
- 아주 먼 곳까지 네트워크를 케이블을 연결할 수는 없다. 이 문제를 처리하기 위해서는 이미 구축된 집에 연결된 전화기 기반 시설을 이용하면 된다. 이 전화기 기반 시설과 네트워크를 연결하기 위해서는 모뎀이 필요하다. 모뎀은 네트워크의 정보를 전화 시설에서 처리할 수 있는 정보로 바꾸는 역할을 한다.

![네트워크-ISP](https://mdn.mozillademos.org/files/8453/internet-schema-7.png)
- 전송 네트워크에서 전달을 받는 네트워크로 메시지를 보내기 위해서는 인터넷 서비스 제공 업체(ISP)에 연결을 해야한다. ISP는 모두 함께 연결되는 몇몇 특수한 라우터를 관리하고 다른 ISP 라우터에도 액세스 할 수 있는 회사이다. 따라서 네트워크의 메시지는 ISP 네트워크의 네트워크를 통해 대상 네트워크로 전달된다. 인터넷은 이러한 구조의 네트워크 인프라로 구성되어져있다.

참고 https://developer.mozilla.org/ko/docs/Learn/Common_questions/How_does_the_Internet_work