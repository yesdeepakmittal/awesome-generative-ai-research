# awesome-generative-ai-research
Generative AI paper summary points

### Gemma 2
- Local(`4096` tokens) & Global(`8192` tokens) Attention in alternate layer
- model variants
   - `2B`(knowledge distillation - *soft labels*✅ | Next Token Prediction - *hard labels*❌ | `26` layers | dense_dim - `2304` | training tokens - `2T`)
   - `9B`(knowledge distillation - *soft labels*✅ | Next Token Prediction - *hard labels*❌ | `42` layers | dense_dim - `3584` | training tokens - `8T`)
   - `27B`(trained from scratch - Next Token Prediction✅ | `46` layers | dense_dim - `4608` | training tokens - `13T`)
- Group Query Attention(`num_groups` - `2`)
- Non-linearity - `GeGLU`
- Vocab size - `256128`
- Context Length - `8192` tokens
- tokenizer - `SentencePiece`
- Post Training - `Supervised fine-tuning (SFT)` & `RLHF`
- Reference - https://arxiv.org/pdf/2408.00118
