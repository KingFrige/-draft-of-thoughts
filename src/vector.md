# vector    

## architecture   

### pipeline

- 独立VectorUnit，与superscalar的EXU分离     
  * 简化rob  

- register bank   

- 独立的VectorUnit & LSU

- 独立的VectorPipe, 与scalar合并的LSU


### vconfig

  加快 `vset{i}vl{i}` 设置速度，可以将vconfig的参数与指令在decode阶段合并到micro-op中，直到commit阶段。

### stripmining 


