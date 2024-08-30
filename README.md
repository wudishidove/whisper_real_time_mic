# whisper_real_time_mic
real time translate voice to text from mic 
及時偵測MIC或喇叭音訊，轉成文本，讓你輕鬆追英V或日V

# 使用教學
## 環境需求
照requirment直接裝，安裝之前記得先裝cuda12.1，因為這份專案用whisper，需要本地顯卡
![](https://medium.com/ching-i/win10-%E5%AE%89%E8%A3%9D-cuda-cudnn-%E6%95%99%E5%AD%B8-c617b3b76deb)
安裝cuda12.1 跟cudnn後，可以直接跑下面的，不然就自己另外裝對應的pytorch
`python.exe -m pip install -r requirements.txt`
## - 1. 安裝 [VB-Virtual Audio Device](https://vb-audio.com/Cable/)
## - 2. 安裝後將CABLE Input設定為預設播放裝置

![image](https://github.com/nKiux/live-JP-CH-translator/assets/46084374/820300ed-2ee2-4ba3-a0ca-e91c96685375)

## - 3. 到錄製，將CABLE output設定為預設裝置，選擇電腦音訊輸出並且將聆聽此裝置勾選，並且將透過此裝置播放選擇為使用中的耳機

![image](https://github.com/user-attachments/assets/ea4700ff-d9b1-42e2-aec4-56bfbc9cf9fc)
![image](https://github.com/user-attachments/assets/58a3a7bb-3a71-46b5-a455-7ee783f368f8)




## - 4. 在同一個資料夾開啟終端機或者CMD(命令提示字元)並輸入下列指令
英文台
`python stable_flex_10_sec.py `
其他語言
`python stable_flex_10_sec.py --non_english`
顯卡很爛想用其他AI模型的話
`python stable_flex_10_sec.py --model tiny`
顯卡很強想用其他AI模型的話
`python stable_flex_10_sec.py --model small`
`python stable_flex_10_sec.py --model medium`
`python stable_flex_10_sec.py --model large`
