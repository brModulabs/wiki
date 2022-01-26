# 목차
- [ready](#ready)
- [segmentation](#segmentation)
- [semantic](#semantic)
- [blur](#blur)
- concat
- problem
# ready
- 사진에서 사람을 찾아서 뽑아내고
- 사람이 없는 사진을 블러 처리한 이후
- 사람을 추가하여 셸로우 포커스(아웃포커스) 효과를 낸다!
# segmentation
- 이미지에서 픽셀 단위로 객체를 추출하는 방식
- 모든 픽셀에 라벨(target)을 할당하여 접근함
## semantic segmentation?
- 사람이 인식하는 것 처럼 인식하는 것을 시맨틱 세그멘 테이션이라고 함
- 물리적인 단위로 분류하는 방법!
## instance segmentation?
- 각 객체들을 따로 인식하자!
## 과거의 segmentation..
- 워터 쉐드 세그멘테이션(satershed segmenttaion)
    - 물체의 경계를 나눠서 찾아냄
    - [관련 링크](https://opencv-python.readthedocs.io/en/latest/doc/27.imageWaterShed/imageWaterShed.html)
# semantic
- FCN, SegNet, U-Net 등 다양하게 존재함
- 그 중 DeepLab V3+를 사용함[관련 링크](https://blog.lunit.io/2018/07/02/deeplab-v3-encoder-decoder-with-atrous-separable-convolution-for-semantic-image-segmentation/)

## [PixelLib](https://github.com/ayoolaolafenwa/PixelLib)
- 다양한 세그멘테이션 모델을 제공한다.
## [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
- 학습 데이터의 종류
- 데이터는 기본적으로 BGR로 저장되어 있음
# blur
- opencv 명령어 사용함
- 이후 마스크의 형상 대로 빈칸을 만듬
