# Vending Machine Test
### source code - [src](https://github.com/PradeeDevananth/CoinProblem/tree/master/VendingMachineTest)
## How to use  
__Download 2 files GUI.exe and VendingMachine.dll__  
[GUI.exe and VendingMachine.dll](https://github.com/PradeeDevananth/CoinProblem/tree/master/VendingMachineTest/GUI/bin/Debug)  

> Self study reference - [My own DataStructure link](https://github.com/DoYourDuty/DataStructure)

## Models
```csharp
    public class ChangeCoin
    {
        public int CoinCount { get; set; }
        public int CoinAmount { get; set; }
    }
    
    public class SellsItem
    {
        public int ItemPrice { get; set; }
        public int ItemCount { get; set; }
        public int ItemNumber { get; set; }
    }

```

__For getting best change coins combinations using below steps__  
1. optimize full combinations of coins list for particular remaining amount
2. Remove duplicate list
3. Remove unavailability coin combinations from list
4. Find ratio of coins from each coin
5. order by less coin ratio to give best combinations of coins
6. Taken from list, less number of coins used combinations
7. Removed from available coins
8. Updated in local DB
