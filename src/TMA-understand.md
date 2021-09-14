TMA understand
================


pipeline & buffer
-------------------

注意：

- pipeline不能跨越buffer，否则便不是同一个pipeline
- pipeline的结果是可预知的


hierarchy
----------



top-down
----------



产生气泡 - bubbles 的原因
---------------------------

- 资源reource不足
   * fetch-buffer
   * fetch-target-queue
   * branchMask
   * issue-slots -> RS
   * rob - entry
   * loadQ
   * storeQ
   * physical registers
   * ALU num
   * decode width
   * fetch width
   * bpd resource

- data dependency
   * read after write dependency

- instruction 
   * branch mispredict
   * branch resteers
   * machine clears


TMA 节点划分的依据与公式的原理
--------------------------------

- pipeline
- buffer


