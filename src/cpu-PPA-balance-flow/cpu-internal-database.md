# cpu internal database


## performance database

### IPC  

### TMAM status

### instruction info

### resource status

### chart  

```json5
{
  IPC: Numbers,
  resource:{
    fetchBufferFull  : Numbers,
    decodeWidthFull  : Numbers,
    branchMaskFull   : Numbers,
    issueSlotsFull   : Numbers,
    exuNumbersFull   : Numbers,
    physicalRegFull  : Numbers,
    robEntryFull     : Numbers,
    loadBufferFull   : Numbers,
    storeBufferEmpty : Numbers,
    fetchBufferEmpty : Numbers,
    decodeWidthEmpty : Numbers,
    branchMaskEmpty  : Numbers,
    issueSlotsEmpty  : Numbers,
    exuNumbersEmpty  : Numbers,
    physicalRegEmpty : Numbers,
    robEntryEmpty    : Numbers,
    loadBufferEmpty  : Numbers,
    storeBufferEmpty : Numbers
  },
  insnInfo:{
    instret   : Numbers,
    cycles    : Numbers,
    intLoad   : Numbers,
    intStore  : Numbers,
    intAmo    : Numbers,
    intSystem : Numbers,
    intArith  : Numbers,
    intBr     : Numbers,
    intJal    : Numbers,
    intJalr   : Numbers,
    intMul    : Numbers,
    intDiv    : Numbers,
    fp        : Numbers,
    fpLoad    : Numbers,
    fpStore   : Numbers,
    fpAdd     : Numbers,
    fpMul     : Numbers,
    fpMadd    : Numbers,
    fpDiv     : Numbers,
    fpOther   : Numbers
  },
  tmam:{
    instret               : Numbers,
    cycles                : Numbers,
    slotsIssed            : Numbers,
    fetchBubbles          : Numbers,
    branchRetired         : Numbers,
    badResteers           : Numbers,
    recoveryCycles        : Numbers,
    fetchNoDeliveredCycles: Numbers,
    brMispredRetired      : Numbers,
    machineClears         : Numbers,
    memStallsAnyLoad      : Numbers,
    memStallsStores       : Numbers,
    uopsDeliveredLe0      : Numbers,
    uopsDeliveredLe1      : Numbers,
    uopsDeliveredLe2      : Numbers,
    exeport0Utilization   : Numbers,
    exeport1Utilization   : Numbers,
    exeport2Utilization   : Numbers,
    exeport3Utilization   : Numbers,
    exeport4Utilization   : Numbers,
    uopsExecutedGe1       : Numbers,
    uopsExecutedGe3       : Numbers,
    noOpsExecutedCycles   : Numbers,
    fewOpsExecutedCycles  : Numbers,
    arithDivider_active   : Numbers,
    memStallsL1Miss       : Numbers,
    memStallsL2Miss       : Numbers,
    memStallsL3Miss       : Numbers,
    issueSlotsEmpty       : Numbers,
    fpRetired             : Numbers,
    iTLBMiss              : Numbers,
    iCacheMiss            : Numbers,
    memLatency            : Numbers,
    unknowBanchCycles     : Numbers
  }
}
```


## area database

### unit area

### all area

### net area 

### chart  

```json5
{
  TopModule:{
   Name: String,
   NetArea:   Numbers,
   cellArea:  Numbers,
   TotalArea: Numbers
  }
  Level1_0: {
   Name: String,
   NetArea:   Numbers,
   cellArea:  Numbers,
   TotalArea: Numbers
  }
  Level1_1: {
   Name: String,
   NetArea:   Numbers,
   cellArea:  Numbers,
   TotalArea: Numbers
  }
  Level2_0: {
   Name: String,
   NetArea:   Numbers,
   cellArea:  Numbers,
   TotalArea: Numbers
  }
}
```




## power database 

### unit power 

  - static power
  - dynamic power 

### system power  

### chart  

```json5
{
  TopModule:{
   Name: String,
   staticPower :  Numbers,
   dynamicPower: Numbers
  }
  Level1_0: {
   Name: String,
   staticPower :  Numbers,
   dynamicPower: Numbers
  }
  Level1_1: {
   Name: String,
   staticPower :  Numbers,
   dynamicPower: Numbers
  }
  Level2_0: {
   Name: String,
   staticPower :  Numbers,
   dynamicPower: Numbers
  }
}
```
