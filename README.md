# UnderstandingTheLayersOfLLMs

##Section 1: 
###Visual Representation of the logits over the layers

##Section 2:
###Consistency check method between these layers for factuality analysis
Consistency checks help identify and correct errors earlier in the process, leading to more accurate results. As we grow in the number of layers, we can maintain the accuracy. By detecting inconsistencies, the approach can reduce the risk of contradictory outcomes. Early exit is a very effective way in understanding the logits development and see if we can find ways on maintaining accuracy. 


##Section 3:
###Layers effect on the metrics 
We can see that with the increase in number of the layers in the model we see some changes to the numbers. The numbers are linear meaning that the model is able to perform better as the layers increase, thereby giving us a better score as the increase in layers.
**Results for different layers used **
| Layer | BLEU | ROGUE-L | BERTScore |
|----------|----------|----------| ----------|
| 8   | 0.00   | 0.01   | 0.74   |
| 16   | 0.00   | 0.01   | 0.75   |
| 24   | 0.00   | 0.06  | 0.78   | 
| 32   | 0.0076   | 0.11  | 0.81   |
