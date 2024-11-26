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

## Visuals
Below is a sample dialogue and its corresponding response with reward values before and after fine-tuning:

| Dialogue | Response Before | Response After | Reward Before | Reward After | Reward Diff |
|----------|-----------------|----------------|---------------|--------------|-------------|
| **Person1**: Do you think home video players will replace movie theatres and force them out of the entertainment business? <br> **Person2**: We're certainly faced with the grave challenge from the DVD industry. That's why I think we have to revolutionize our concept of movie showing. As I see it, the movie theatre should not just be a place to watch a film, but a place to meet people. | #Person1# thinks home video players will replace movie theatres, but does not expect them to create technological changes. | The DVD industry has gone downhill in recent years, forcing home video players out of the entertainment industry. | 0.967161 | 4.708010 | 3.740849 |

After fine-tuning, the model produces more refined and meaningful responses, as reflected in the higher `not hate` reward, showcasing its enhanced ability to generate positive, high-quality content.
```python
After fine-tuning, the model produces more refined and meaningful responses, as reflected in the higher `not hate` reward, showcasing its enhanced ability to generate positive, high-quality content.
```

