# vector    

## architecture   


### pipeline

- 融合到superscalar之中，在decode阶段将vector指令分解为多个scalar操作
   * 增大issue width       
   * 复用registerfile     
   * ROB commit做区分处理， 复杂   

- 独立VectorUnit，与superscalar的EXU分离     
  * 简化rob  

- 独立的VectorUnit & LSU

- 独立的VectorPipe, 与scalar合并的LSU


### vconfig

  加快 `vset{i}vl{i}` 设置速度，可以将vconfig的参数与指令在decode阶段合并到micro-op中，直到commit阶段。

### stripmining & 指令fuse/package

The base "V" vector extension requires that VLEN≥128.

The value of 128 was chosen as a compromise for application processors. Providing a larger VLEN allows stripmining code to be elidedin some cases for short vectors, but also increases the size of the minimum implementation. Note that larger LMUL can be used toavoid stripmining for longer known-size application vectors at the cost of having fewer available vector register groups. For example,an LMUL of 8 allows vectors of up to sixteen 64-bit elements to be processed without stripmining using four vector register groups.

因为VLEN >= 128，当VLEN为256/512/...，大于128时，编译器假设默认参数VLEN=128,以获得更好的兼容性，如何在VLEN > 128的微架构上获得更好的性能呢？

或许使用指令融合的方面，解析多条相同操作的指令，merge到一个发射槽之中，修正vconfig参数。




