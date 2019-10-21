Chinese Medical Intent Dataset(CMID)
====

This dataset is used for Chinese medical QA intent understanding task.

More details will be updated soon.

Dataset format:
======
All the data is stored in a JSON file. There are 5 fields in the file. An example as follows:

    {
     "originalText": "间质性肺炎的症状?", 
     "entities": [{"label_type": "疾病和诊断", "start_pos": 0, "end_pos": 5}], 
     "seg_result": ["间质性肺炎", "的", "症状", "?"], 
     "label_4class": ["病症"], 
     "label_36class": ["相关病症"]
    }

The field details
-------
The "originalText" field holds the input information.
The "entities" field holds the Named entity recognition information with Deep learning model. The tag of the entity follows the CCKS2019 Task1 standard:https://www.biendata.com/competition/ccks_2019_1/Evaluation/.
The "seg_result" field holds the information after sentence segmentation.
The "label_4class" field holds the manually annotated medical intent classification information.
The "label_36class" field holds the manually annotated medical intent classification information.
