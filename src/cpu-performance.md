cpu performance
===================

- structural hazards
- data hazards
- control hazards(branch, exceptions)


bubbles analysis
------------------

- commit  bubbles  -> rob
- issue  bubbles   -> issuleQ
- frontEnd bubbles -> fetchBuffer


hazards analysis
-------------------

- decode hazards
- dispatch hazards


resource analysis
-------------------

- state
  * empty
  * full

- fetch buffer
- issueslots
- lsu: ldq/sdq/saq
- rob
- rename stage:phy-register/freelist
- branchTags

- register file ports
- alu ports


top-down summarize
----------------------

- top-down method accomplish
  * events & counters define
  * debug

- top-down hierachy framewaork

- data collection & analysis 
  * benchmarks porting: coremark/spec2006Int

- improve design


the strategies for data hazards
--------------------------------

- interlock
- bypass
- speculate
  * branch prediction


