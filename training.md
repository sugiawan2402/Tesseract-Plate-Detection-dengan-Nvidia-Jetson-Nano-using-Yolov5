python train.py --img 416 --batch 16 --epochs 30 --data ../helm/data.yaml --weights yolov5s.pt --cache
python train.py --img 416 --batch 16 --epochs 30 --data ../full/data.yaml --weights yolov5s.pt --device 0
python train.py --img 416 --batch 16 --epochs 10 --data ../parking/data.yaml --cfg ./models/yolov5s.yaml --weights yolov5s.pt --name yolov5s_results  --cache

#run
python .\detect.py --weights .\runs\train\exp52 \weights\last.pt --source 0

python .\detect.py --weights ppe3.pt --source 0