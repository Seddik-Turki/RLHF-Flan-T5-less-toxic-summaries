# RLHF-Flan-T5-less-toxic-summaries

## Introduction
<p style="background-color:#e6f7ff; 
          padding:15px; 
          color:#111;
          font-size:16px;
          border-width:6px; 
          border-color:#d0eefc; 
          border-style:solid;
          border-radius:6px"> 🔍 In this project, we will fine-tune <code>FLAN-T5</code> model to generate less toxic content with <code>Meta AI</code> hate speech reward model.</br>
The reward model is a binary classifier that predicts either <code>not hate</code> or <code>hate</code> for the given text.</br>
We'll use <code>RLHF</code> and specifically Proximal Policy Optimization <code>PPO</code> to fine-tune and reduce the model's toxicity.
</p>

