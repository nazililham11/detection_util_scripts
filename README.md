# Object detection utility scripts

original : https://github.com/douglasrizzo/detection_util_scripts

## Usage

* **generate_csv.py** 
```
python generate_csv.py \
	--type=xml \
	--input=object-detection/train \
	--output_csv=train.csv \
```


* **generate_train_eval.py**
``` 
python generate_train_eval.py \
	--type=xml \
	--input=object-detection/train \
	--output_csv=train.csv \
```


* **generate_pbtxt.py** 
```
python generate_pbtxt.py \
    --input_type=csv \
    --input_file=output.csv \
    --output_file=labelmap.pbtxt
```


* **generate_tfrecord.py** 
```
python generate_tfrecord.py \
    --csv_input=output.csv \
    --pbtxt_input=labelmap.pbtxt \
    --image_dir=images \
    --output_path=output.tfrecord
      
```