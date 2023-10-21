# SOC-Design-Lab3
Simulation log檔案是用Xim的方式模擬出來的
Waveform裡共有4個圖檔，分別是
  coeffic_input.png ： 標示h[i]資料(tap parameter)從AXI-write protocol進入fir design同時顯示tap Bram將此資料存進Bram的data flow
  coeffic_output.png ：標示h[i]資料(tap parameter)從AXI-read protocol讀回fir testbench同時顯示tap Bram將此資料讀出Bram的data flow
  ap_start.png ：      fir testbench送ap_start後 fir design開始運作，並同時顯示tap Bram與data Bram存取資料的data flow
  ap_done_and_next.png ： fir design結束他的運算後，fir testbench去檢查ap_done與ap_idle，確認無誤後送下一筆data計算的ap_start flag
