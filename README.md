# 🏆 마스크 착용 상태 분류 대회

![image](https://user-images.githubusercontent.com/91870042/156874151-4d1c362b-bae6-4781-8064-315d12d3ba60.png)

> COVID-19의 확산으로 우리나라는 물론 전 세계 사람들은 경제적, 생산적인 활동에 많은 제약을 받고있습니다. 확산 방지를 위해 많은 노력들을 하고 있지만 COVID-19의 강한 전염력 때문에 우리를 오랜 기간 괴롭히고 있습니다. </br>
> 감염 확산 방지를 위해 무엇보다 중요한 것은 모든 사람이 마스크로 코와 입을 가려서 전파 경로를 원천 차단하는 것입니다. </br>
> 이를 위해 우리는 공공장소에서 모든 사람들의 올바른 마스크 착용 상태를 검사하는 시스템이 필요합니다. </br>
> 즉, **카메라로 비춰진 사람 얼굴 이미지만으로 이 사람이 마스크를 쓰고 있는지, 쓰지 않았는지, 정확히 쓴 것이 맞는지 자동으로 가려낼 수 있는 시스템이 필요합니다.**

## 📅 기간
**대회 진행**: 2022년 2월 21일 10:00 ~ 2022년 3월 3일 19:00  


## 💯 Evaluation
<img src="https://user-images.githubusercontent.com/97524127/171376238-48e34af9-5dc1-4e00-8fe4-cc01ed81407d.png"  height="200"/>

## 🌟 Result
![image](https://user-images.githubusercontent.com/97524127/171377368-4aa70cec-f2e0-441f-a53c-405c6a42558d.png)

## 📁 Dataset   
- 전체 사람 명 수 : 4500명 (train : 2700 | eval : 1800)
- age : 20대 ~ 70대
- gender : 남, 여
- mask : 한 사람 당 정상 착용 5장, 이상하게 착용 1장(코스크,턱스크), 미착용 1장
- 이미지 크기 : (384, 512)

**Class Description**
- mask, gender, age 기준 18개의 클래스로 분류
<img src="https://user-images.githubusercontent.com/68593821/131881060-c6d16a84-1138-4a28-b273-418ea487548d.png" height="500"/>

## 💡 Model  
- **ResNet 18**
- Loss: Focal Loss
- Optimizer: Adam
- Hyperparameter
  - Batch Size: 64
  - Epoch: 5
  - Learning Rate: 0.0001
