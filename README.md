# DQN, DDQN을 활용한 LunarLander-v2(discrete) 학습 
 
### 1) 학습 결과(모델) 
   - https://drive.google.com/drive/folders/1ctDUQR4CuaUw_hy1WiQizPQn64YdYS3l?usp=sharing
#
### 2) 설치 라이브러리
#### !pip install opencv-python
#### !pip install gym[all,accept-rom-license]
#### !pip install swig
#### !pip install --upgrade pip setuptools wheel
#### !pip install --upgrade gym
#### !pip install tqdm
#### !pip install gym[box2d]
#### !pip install pandas
#
### 3) 실험환경
- 실험 환경 (Experiment Environment)
   - Environment : LunarLander-v2
   - Action Space: 이산적인 4가지 액션 (0부터 3까지)
   - State : 8차원 벡터로 표현된 우주선의 상태
   - Rewards : 각 단계에서 제공되며, 착륙 지점에 가까우면 증가하고 멀어지면 감소함            
                      추가적인 보상 및 패널티는 충돌 및 안전한 착륙에 대한 것도 있음
 - 데이터셋 (Dataset)
   - 개별적인 데이터셋이 명시적으로 제공되어 있지 않음
 - 목표
   - 안전하게 착륙 시키면서 최대한 많은 보상을 얻도록 학습 시키는 것
   - 최종 목표는 agent가 episode별로 적어도 200점 이상의 누적 reward를 얻는 것

