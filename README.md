# Mediapipe examples using uv

## Installation

```
python 3.9
git clone https://github.com/ligaoqi2/Mediapipe-examples-using-python-uv.git
uv sync
uv pip install tensorflow
```

For the iris example, put `iris_landmark.tflite` into `models` directory, by unpacking following zip file:
```
https://github.com/google/mediapipe/files/10012191/iris_landmark.zip
```

The facial expression example uses the trained weights from [github.com/zengqunzhao/EfficientFace](https://github.com/zengqunzhao/EfficientFace), but converted to tflite.
For the facial expression example download both models (fast and slow) into the `models` directory:

```
wget -P models https://rassibassi-mediapipedemos.s3.eu-central-1.amazonaws.com/efficient_face_model.tflite
wget -P models https://rassibassi-mediapipedemos.s3.eu-central-1.amazonaws.com/dlg_model.tflite
```

## Run

One of the following:

```
python facial_expression.py
python face_detection.py
python face_mesh.py
python hands.py
python head_posture.py
python holistic.py
python iris.py
python objectron.py
python pose.py
python selfie_segmentation.py
```

`pose.py` and `iris.py` include the possibility to process a video file instead of the webcam input stream. Run like this:

```
python iris.py -i /path/to/some/file/i-am-a-video-file.mp4
python pose.py -i /path/to/some/file/i-am-a-video-file.mp4
```

## Numpy

See example `python pose.py` for how to extract numpy array from the mediapipe landmark objects.

## Acknowledgements
```
https://google.github.io/mediapipe/
https://github.com/Rassibassi/mediapipeDemos
```

### Contact
```
ligaoqi02@gmail.com
```
