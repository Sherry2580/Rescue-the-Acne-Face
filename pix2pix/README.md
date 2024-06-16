# Pix2Pix_official
## Workflow
- **Add simulation Acne**: `noise.ipynb`
- **Train & Test pix2pix model**: `pix2pix.ipynb`

## Preprocess data
`noise.ipynb`檔案內有許多cell，分別是:
1. **Add acne to face**: 
2. **Cut and resized images**:
3. **Resized images**:
4.


## 標記資料欄位說明

- **x**: 物件中心 x 位於整張圖片寬度的比例。
- **y**: 物件中心 y 位於整張圖片高度的比例。
- **w**: 物件的寬度，佔整張圖片寬度的比例。
- **h**: 物件的長度，佔整張圖片長度的比例。
- **conf**: YOLO 偵測到痘痘的機率，我把大於0的全部output了，可以自己設定threshold~

詳細說明可參考 [這篇文章](https://blog.cavedu.com/2019/07/25/yolo-identification-model/)。


## Conf 挑選

- **原始照片**  
<img src="example/levle0_1.jpg" width="30%">

- **conf > 0.01**:  
<img src="example/levle0_1_0.01.jpg" width="30%">

- **conf > 0.1**:  
<img src="example/levle0_1_0.1.jpg" width="30%">

- **conf > 0.2**:  
<img src="example/levle0_1_0.2.jpg" width="30%">
