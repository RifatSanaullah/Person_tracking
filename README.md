##Person Tracking demo!!

This tracking demo video based on bytetrack algorithm to track person based on video frame.
I used bytetrack_x_mot17.pth.tar pretrained model to inference the video.
Added some custom logic to draw a line and count the person in and out from the line.

I added requirements.txt file and necessary library to infer the video.
absl-py==2.1.0
colorama==0.4.6
contourpy==1.3.1
cycler==0.12.1
Cython==3.0.11
cython-bbox-og==1.0.0
filelock==3.16.1
filterpy==1.4.5
fonttools==4.55.0
fsspec==2024.10.0
grpcio==1.68.0
h5py==3.12.1
imageio==2.36.0
Jinja2==3.1.4
kiwisolver==1.4.7
lapx==0.5.11
lazy_loader==0.4
loguru==0.7.2
Markdown==3.7
MarkupSafe==3.0.2
matplotlib==3.9.2
motmetrics==1.4.0
mpmath==1.3.0
networkx==3.4.2
ninja==1.11.1.1
numpy==1.26.4
opencv-python==4.10.0.84
packaging==24.2
pandas==2.2.3
pillow==11.0.0
protobuf==5.28.3
pycocotools==2.0.8
pyparsing==3.2.0
python-dateutil==2.9.0.post0
pytz==2024.2
scikit-image==0.24.0
scipy==1.14.1
six==1.16.0
sympy==1.13.1
tabulate==0.9.0
tensorboard==2.18.0
tensorboard-data-server==0.7.2
thop==0.1.1.post2209072238
tifffile==2024.9.20
torch==2.5.1+cu124
torchaudio==2.5.1+cu124
torchvision==0.20.1+cu124
tqdm==4.67.0
typing_extensions==4.12.2
tzdata==2024.2
Werkzeug==3.1.3
win32-setctime==1.1.0
xmltodict==0.14.2


I used python version 3.11.8

Device Configuration:
ryzen 7 5700x
nvidia rtx 3070


To inference the code:
python demo_track.py video --path 'D:/ByteTrack/Computer Vision task Culture Hint.mp4' -f exps/example/mot/yolox_x_mix_det.py 
-c D:/ByteTrack/bytetrack_x_mot17.pth.tar --fp16 --fuse --save_result --device gpu


