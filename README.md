# UnderstandingTheLayersOfLLMs

## How to run the notebook:
- First make sure to have gpu access
- Open the notebook
- Run all the cells

## Section 1: 
### Visual Representation of the logits over the layers
- See graph.png file
- We notice that after layer 8 the generation is very bad and the results is considered to be zero accuracy. Similarly for layers 16 and 24 too not much considerable changes are to be seen in the accuracy. After layer 32 we see the model being able to handle the generation well so that the accuarcy reaches to about 80% for the predictions on a test set. This graph also shows that the learning is changing substantially even after the upper layers i.e 24+ layers and with only 1/2 layers at towards the 32nd layer the results change well. 

## Section 2:
### Consistency check method between these layers for factuality analysis
Consistency checks help identify and correct errors earlier in the process, leading to more accurate results. As we grow in the number of layers, we can maintain the accuracy. By detecting inconsistencies, the approach can reduce the risk of contradictory outcomes. Early exit is a very effective way in understanding the logits development and see if we can find ways on maintaining accuracy. 


## Section 3:
### Layers effect on the metrics 
We can see that with the increase in number of the layers in the model we see some changes to the numbers. The numbers are linear meaning that the model is able to perform better as the layers increase, thereby giving us a better score as the increase in layers.

**Results for different layers used**
| Layer | BLEU | ROGUE-L | BERTScore |
|----------|----------|----------| ----------|
| 8   | 0.00   | 0.01   | 0.74   |
| 16   | 0.00   | 0.01   | 0.75   |
| 24   | 0.00   | 0.06  | 0.78   | 
| 32   | 0.0076   | 0.11  | 0.81   |
