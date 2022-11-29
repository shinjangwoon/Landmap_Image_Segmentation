# Landmap_Image_Segmentation
## 항공사진을 이용한 토지피복지도 객체 분할

이미지 (CV) | 개방형 문제 | mIoU

문제정의

• 주어진 항공사진 속에 픽셀들이 건물인지 아닌지 이미지를 분할하는 문제

![image](https://user-images.githubusercontent.com/83771596/204474535-6d652bc5-5313-481f-bc9e-1ed9272a52ec.png)

![image](https://user-images.githubusercontent.com/83771596/204474412-b5445358-7ddb-4686-ba12-e3d0d7215282.png)

```sh
<데이터 상세>

Input

- 512 x 512 크기의 항공/위성사진

- .png 형태

Target

- 512 x 512 크기의 마스크

- .png 형태

수량

- n_train = 3930

- n_test = 1303

<데이터 디렉토리 구조>

DATA/

├── train/

│         ├── traindf.csv  

│         ├── images/

│         │        ├── xxx.png

│         │        ├── yyy.png

│         │        ├── zzz.png

│         │        └── ...  

│         └── masks/

│                      ├── xxx.png

│                      ├── yyy.png

│                      ├── zzz.png

│                      └── ...  

└── test/

             ├── sample_submission.csv

             ├── testdf.csv

             └── images/

                          ├──  aaa.png

                          ├──  bbb.png  

                          └──   ...



```
