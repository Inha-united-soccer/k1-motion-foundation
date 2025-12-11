# k1-motion-foundation

## k1-motion-foundation
Booster K1의 기본 동작을 단계적으로 구축하기 위한 레포지토리입니다.

Walk, Kick, Pass와 같은 핵심 동작들부터 구현될 예정이며 각 동작은 개별 브랜치에서 개발 후 Pull Request를 통해 병합될 예정입니다.  
</br>

## Initial Behavior Setting

k1 드리블 동작을 구현하기 위해 `dribble.xml`에서 BehaviorTree 노드들이 조합됩니다.</br>
</br>
초기 구현 단계에서 사용되는 동작들은 다음과 같습니다. 

| 구분 | 노드 이름 | 역할 설명 |
|-----------|-----------|-----------|
| **공 추격** | SimpleChase | 탐지된 공을 향해 나아가는 동작 |
| **직진 드리블** | SetVelocity | 로봇에 직진 속도를 부여함으로써 드리블을 구현 |
| **공 추적** | CamTrackBall | 카메라를 통해 공을 추적 |
| **공 탐색** | CamFindBall | 공이 시야에 없을 때 탐색 동작 구현 |
| **필드 스캔** | CamScanField | 경기장을 스캔하는 동작 |
</br>

이후 추가되는 모든 동작들은 하드웨어를 통해 검증된 후 추가될 예정이며 commit log를 통해 확인할 수 있습니다.

