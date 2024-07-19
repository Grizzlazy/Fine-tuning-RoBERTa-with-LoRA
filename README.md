# Fine tuning RoBERTa with LoRA
Using LoRA in the Query and Value in the Attention layers

Base model param count: 125237762

Model with LoRA param count: 589824, 212 times smaller than base model

**Average time per epoch**
- Without LoRA: 23 minutes 36 seconds
- With LoRA: 17 minutes 1 seconds

**Test set Accuracy**
- Without LoRA: 96.31%
- With LoRA: 95.51%

While being 200x smaller than the base model, the LoRA model is about 25% faster during fine-tuning, and has a test set accuracy of 95.51% compared to 96.31% of the base model, after 3 epochs of training.
