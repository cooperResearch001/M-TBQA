# M-TBQA
The dataset for M-TBQA

1、Dataset.

Our dataset consists of 1000 tables, primarily sourced from Baidu Baike and real e-commerce scenarios, with 5000 manually annotated questions. The researchers can download this dataset for the experiment of multimodal table-based question answering. The data will be open-sourced in JSON format as follows:
```json
{"rows": [["飞科", "使用问题", "怎么开机", "https://img11.360buyimg.com/ddimg/jfs/t1/103598/39/15069/1071568/5e6ddf28Ef5f8d3b2/5bc73ed2cc3af493.jpg"], 
["耐克", "换货", "有点小", "https://img11.360buyimg.com/ddimg/jfs/t1/100809/6/17078/207734/5e832809E99734b44/18589730bc55d86e.jpg"]],
"name_id": "1",    
"title": "品牌客户投诉 ",    
"header": ["品牌", "客户诉求", "存在问题", "img"],  
"types": ["str", "str", "str", "url"],     
"question": "耐克需要换货的商品是什么颜色?",  
"answer": "黑色",
"aggregation": [NONE],
"select_rows": [2],
"select_columns": [3]
}
```
| json element | description |
|  ----  | ----  |
| rows | table content |
|  name_id  | table  |
|  title  | table title  |
|  header  | table header  |
|  types  | `str` represents string data type, `int/float` represents numerical data types, and `url` represents an image  |
|  question  | labeled question  |
|  answer  | labeled answer  |
|  aggregation  | aggregation operator  |
|  select_rows  | which rows are selected |
|  select_columns  | which columns are selected |

2、Notice.

Since some of the data is sourced from real e-commerce scenarios, the data will be open-sourced after manual review and assessment to mitigate potential ethical and legal risks.

The resources related to this project are intended for research and academic purposes only, and they are strictly prohibited for commercial use. Anyone who uses this dataset for commercial purposes should be responsible for any legal risks that may arise.
