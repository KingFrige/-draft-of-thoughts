# vector    

## architecture   

- 融合到superscalar之中，在decode阶段将vector指令分解为多个scalar操作
   * 增大issue width       
   * 复用registerfile     
   * ROB commit做区分处理， 复杂   

- 独立VectorUnit，与superscalar的EXU分离     
  * 简化rob  

