# AIHUB_PROJECT_MODEL

<h2>확인 바랍니다.</h2>
$$ 최종 Best Weight file의 용량이 깃허브 허용보다 큰 관계로 구글 드라이브에 저장했습니다. 다운 받아 확인해주시면 감사드리겠습니다 :) <br>
https://drive.google.com/file/d/1zYl4nPQaFjkHT2IE5jiQbmetFkHGz7B9/view?usp=sharing  <br>

<h2>코드 동작 관련 설명입니다.</h2>
<span>
  # bypy_best.pt 다운로드 후 ./weights 경로에 저장 부탁드립니다. <br>
  # hyperparmeter 및 translation 등 augmentation에 필요한 hyps 수정 코드 ./data/hyps/hyp.scratch.yaml <br>
  # datapath 코드 ./data/bypy.yaml <br>
  # image, labels 분류 및 처리 코드 ./sorting.ipynb <br><br>
  # training code <br>
  !python train.py --img 480 --batch {batch} --epochs {epochs} --data ./data/bypy.yaml --weights ./weights/bypy_best.pt --name {model_name} <br>
  # runs/train/model_name 경로에 weight와 results 저장 <br><br>
  # evaluation code <br>
  !python detect.py --weights ./weights/bypy_best.pt --source {source_file_path} --conf-thres {confidence_threshold} <br>
  # runs/detect/exp 폴더에 results 저장 <br>
</span>
