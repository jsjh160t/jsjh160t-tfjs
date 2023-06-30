# jsjh160t.github.io/jsjh160t-tfjs

01/啟動TF demo<br>
02/Template Image Classification ：本地端範例(tiger.jpg) cat<br>
03/Custom Image Classification  ：無法上傳檔案(20230624解決--自訂上傳按鈕)(chatgpt)<br>
04/Template Image Object Detection ：本地端範例(od_sample4.jpg)<br>
05/WebCam Image Object Detection  無法擷取影像(20230624解決--將google.colab那一行註解掉)<br>
06/WebCam Video Object Detection<br>
07/Template Image 人體姿態(靜態) ：本地端範例(pose_sample2)-firefox可以，chrome不行<br>
  (20230627增加以下指令，就可以在chrome正常執行。)(chatgpt)<br>
  // 觸發函式<br>
  async function loadImage(e) {<br>
     //方法1.等待~~確保 TensorFlow.js 在進行其他操作之前已經初始化。<br>
     await tf.ready();<br>
     //方法2.等待 TensorFlow.js 初始化，確保後端已經設置好並且準備就緒。<br>
     //await tf.setBackend('webgl'); <br>   
        
08/Custom Image 人體姿態(靜態) ：無法上傳檔案(20230624解決--自訂上傳按鈕)(chatgpt)<br>
  (20230627增加同上指令，就可以在chrome正常執行。)(chatgpt)<br>

09/WebCam Image 人體姿態(動態) ：無法擷取影像<br>
  (20230627增加以下指令，就可以在chrome正常執行。)(chatgpt)<br>
  // webcam 攝影<br>
  async function takePhoto() {<br>
    //方法1.等待~~確保 TensorFlow.js 在進行其他操作之前已經初始化。<br>
    //await tf.ready();<br>
    //方法2.等待 TensorFlow.js 初始化，確保後端已經設置好並且準備就緒。<br>
    await tf.setBackend('webgl');<br>
    
10/WebCam Video 人體姿態(動態) ：無法顯示<br>
  (20230630增加以下指令，就可以在chrome正常執行。)(chatgpt)<br>
  async function app() {<br>
    //方法1.等待~~確保 TensorFlow.js 在進行其他操作之前已經初始化。<br>
    //await tf.ready();<br>
    //方法2.等待 TensorFlow.js 初始化，確保後端已經設置好並且準備就緒。<br>
    await tf.setBackend('webgl');<br>
        
11/Custom Image 多人人體姿態(靜態) ：無法上傳檔案(20230630解決--自訂上傳按鈕)(chatgpt)<br>
  (20230630增加以下指令，就可以在chrome正常執行。)(chatgpt)<br>
  // 觸發函式<br>
  async function loadImage(e) {<br>
     //方法1.等待~~確保 TensorFlow.js 在進行其他操作之前已經初始化。<br>
     await tf.ready();<br>
     //方法2.等待 TensorFlow.js 初始化，確保後端已經設置好並且準備就緒。<br>
     //await tf.setBackend('webgl'); <br>   

tmo~tm2：teachable machine的models+javascript，tm0：沒照HTML格式規範，tm1：(原始版)webcam+修改檔案來源，tm2：chatgpt改為上傳檔案並清除預測值+tf.ready()

