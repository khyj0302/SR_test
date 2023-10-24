# synthetic dataset USAGE


.csv File description
---------------------
1. Month/data.CSV : Original_name / New_name / decayed_id
2. Mapping_key_M/D.csv : 내부키 / 충치번호 / 제출용 키


Mapping JSON
---------------------
1. Check Original_name

2. find New_name with Original_name in M/D.csv<br/>
　(ex)<br/>
　Original_name: 405_lower_34_v1_mola2_examples_NOT_EMA_epoch=000133.ckpt.png <br/>
　New_name: 1011_405_lower_99_datasetv2_decayedSDIv1_7.png<br/>
3. New_name is 내부키<br/>
　(ex)<br/>
 　New_name : 1011_405_lower_99_datasetv2_decayedSDIv1_7.png<br/>
 　내부키: 1011_405_lower_99_datasetv2_decayedSDIv1_7<br/>
3. find 제출용키 with New_name<br/>
(ex)<br/>
 　내부키: 1011_405_lower_99_datasetv2_decayedSDIv1_7 <br/>
 　제출용키: lower_2725<br/>
6. 제출용키 is Json file name. (find the json file in label_json folder)
