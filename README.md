Nhận diện khuôn mặt khá chuẩn xác bằng MTCNN và Facenet!

Article link: http://ainoodle.tech/2019/09/11/face-recog-2-0-nhan-dien-khuon-mat-trong-video-bang-mtcnn-va-facenet/


python3 src/align_dataset_mtcnn.py  Dataset/FaceData/raw Dataset/FaceData/processed --image_size 160 --margin 32  --random_order --gpu_memory_fraction 0.25

python3 src/classifier.py TRAIN Dataset/FaceData/processed Models/20180402-114759.pb Models/facemodel.pkl --batch_size 1000

python3 src/face_rec_cam.py


python3 src/face_rec.py --path video/nguyenthihongthuy.mp4 