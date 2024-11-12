# Stereo-Depth

이 프로젝트는 두 개의 카메라를 통해 얻은 이미지에서 physical space의 한 point에 대한 disparity를 구함으로써 depth를 추정합니다.

## 프로젝트 파일 구조

### 필요한 파일들

- **requirements.txt**: Stereo depth 계산을 위해 필요한 라이브러리와 그 버전 정보를 담고 있습니다. 다음 명령어로 필요한 라이브러리들을 설치할 수 있습니다.
  ```bash
  pip install -r requirements.txt

- **stereo_set**: 왼쪽, 오른쪽 시각의 사진 2장

## 학습 코드

- **HW3 Stereo Depth Calculation.ipynb**:  
  왼쪽, 오른쪽 두 시각의 이미지를 통해 disparity map을 계산하여 각 픽셀의 disparity 값을 얻고, 이를 기반으로 depth 정보를 추정합니다.
  
- **HW3 Stereo Depth Calculation_Change Parameter.ipynb**:  
  HW3 Stereo Depth Calculation.ipynb의 commpute_left_disparity_map 함수에서 num_disparities, block_size, window_size를 변화시킨 후 depth 정보를 추정합니다.

- **files_management**: 왼쪽 및 오른쪽 카메라의 투영 행렬을 정의 & stereo 처리에 필요한 좌우 이미지를 로드하는 함수 & 왼쪽 이미지에서 장애물 이미지를 잘라내는 함수

## 결과
- HW3 Stereo Depth Calculation.ipynb, HW3 Stereo Depth Calculation_Change Parameter.ipynb 안에 결과 사진이 있습니다.
