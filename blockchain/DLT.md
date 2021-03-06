# 분산원장기술

---

## DLT란

- DLT(Distributed ledger Technology)
  분산 원장 기술

중앙원장기술과 반대로 중앙서버나 중앙관리자의 제어 없이 분산화된 네트워크의 각 노드(개인)들이 데이터베이스를 공유하고 계속 동기화하는 기술입니다.

> 중앙원장기술이란
>
> - 기존의 은행이나 시스템과 같이 모든 데이터가 중앙집중의 형태로 되어있는 방식.
> - 이는 중앙시스템관리자가 알아서 잘 관리하고 처리해줄 것이라는 신뢰가 뒷받침되어 있음

그러면 분장원장기술이랑 블록체인이랑 뭐가 다른 걸까?

이에 대한 대답은 _"모든 블록체인은 분산 원장이지만 모든 분산 원장이 블록체인인것은 아니다"_
라고 할 수 있습니다.

블록체인은 분산원장의 기술들 중 하나로 블록이라는 단위를 사용하여 시간의 연속을 구성하는 기술입니다.
블록에는 해쉬함수를 통해 해쉬화된 데이터가 들어가며 이 블록들이 연결되어 체인을 이룹니다.
그리고 이렇게 구성된 블록체인은 하나의 원장으로서 분산되어있는 모든 노드들에 복제, 공유되어 모두가 사본을 관리하고 동기화합니다. 그렇게 P2P네트워크를 구현하고 데이터가 변경될 때마다 검증노드에서 검증하여 신뢰성 높은 블록체인을 구성하는 것입니다.
