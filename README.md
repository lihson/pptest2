# 2023 ADL HW2
Author: 栗漢文  r11922191 

## Training
1. Make sure the datas like train.jsonl, public.jsonl and are already locate in `./data/`
2. Train the mt5-small Summrization model by:
   ``` shell
   sudo bash ./train.sh
   ```
   The train.sh contains only one step:
   * run train.py to train a Summrization model
      
   The hyper-parameters in train.sh can be modified  
   The model will locate in `./ckpt`

## Testing
1. Download the model I trained by:
   ``` shell
   sudo bash ./download.sh
   ```  
2. Test the model by:
   ``` shell
   sudo bash ./run.sh /path/to/input.jsonl /path/to/output.jsonl
   ```

## Others
1. The code for ploting for Report Q2 are already embeded in train.py.  
2. run_strategy.sh and test_strategy.py are for the Report Q3.
