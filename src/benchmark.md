# benchmark

## what is a benchmark?   
## Why use a benchmark?   

## performance


- freq - f
- period - t
   
   t = 1/f

- 性能 = 1 / 执行时间

- CPI

   CPI = CPU时钟周期数 / 指令数


## coreMark

coreMark = 迭代次数 / 执行时间 = 迭代次数 / （每次执行时间 * 迭代次数）= 1 / 每次执行时间 = IPC * Cont-coremark
         = 1 / （Num-Insn * CPI * 时钟周期时间） = 时钟频率 / （Num-Insn * CPI）= IPC * 时钟频率 / Num-Insn

         -> coreMark = IPC * 时钟频率 / Num-Insn


## benchmark suite

- spec2006     
- spec2017    
- whisper   
- Whetstone   
- NAS Parallel Benchmarks   
- LINPACK    
- LAPACK    
- Lawrence Livermore Loops    
- dhrystone    
- coremark     
- 3Dmark06   
- SPEC viewperf 9.0   
- 3D games   
- CommBench  
- PacketBench   


## How to design a benchmark?  

## reference
