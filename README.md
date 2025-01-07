<h1 align="center"> MoEVilbert </h1>

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/7e4e98f8-8b35-44d2-8c7b-4e45bcfa16ff" alt="image" width="700">
</p>

<br>




---

**Architecture of MoEVilbert**  

MoEVilBERT extends the single-task ViLBERT model by incorporating expert models as its base. The outputs from these experts are fused and passed to task-specific networks. A critical component of the model is the gating network, which dynamically generates weights based on input to combine embeddings from each expert. The final embedding is a weighted sum of the expert outputs.  

The model consists of 860,386,003 parameters in total, with only 10,723,795 trainable parameters. This low ratio is achieved by freezing a significant portion of the parameters, including those of the experts.  

