# Delegate Incoming Monitor (DIM)
A tool to collect data from all blocks forged by a delegate in a certain time period, including the value per block in BTC/USD/EUR at the time of forging. Useful for tax purposes, for example.

If you like this software, please consider a donation =] `6725360537423611335L`

## Usage
DIM can be run "as-is" in interactive mode, or with optional arguments.

#### Interactive Mode
Open `dim.exe` and follow the instructions.

#### Arguments
DIM accepts multiple (optional) arguments. Examples are:

`dim.exe --network testnet --address 7134531444980378449L`

`dim.exe --network mainnet --address 13943256167405531820L --start 2018/09/01 --end 2018/09/10`

For a complete list, please see:
``` .\dim.exe -h

optional arguments:
  -h, --help            show this help message and exit
  --network {mainnet,testnet,custom}
                        use 'mainnet' or 'testnet'
  --address ADDRESS     specify delegate address
  --start START         specify start date (yyyy/mm/dd)
  --end END             specify end date (yyyy/mm/dd)
```  
#### Running the Python script
You can run the original Python script if that's preferred. The only non-standard library used is `requests`, found in the `requirements.txt` file. All of the above instructions still apply to using this method.