## About SFL-PDA (abstract of our work)
Self-supervised federated learning can leverage unlabeled data to alleviate representation-level data heterogeneity but remains limited in addressing label-level imbalance. While pre-trained generative models show promise for augmenting minority-labelled data, their effectiveness diminishes in real-world FL scenarios, where client data is private and must not be exposed to the public. To fill this gap, we propose SFL-PDA (*Self-supervised Federated Learning with Personalized Diffusion Adapter*) to address data heterogeneity at both representation- and label-levels. SFL-PDA designs a lightweight class-conditioned LoRA adapter to finetune a personalized diffusion model as per client requests. In this way, the client’s diffusion model can effectively capture private, domain-specific characteristics for personalized minority-class data generation, ensuring SFL is collaboratively trained with balanced labeled data and achieves consistent performance.  We evaluate SFL-PDA on two standard benchmarks and one private domain-specific dataset against various state-of-the-art baselines under varying heterogeneity levels. The results demonstrate that SFL-PDA can effectively address data heterogeneity, especially at severe levels. Furthermore, ablation studies confirm that our proposed class-conditioned LoRA adapter can yield up to 28.5% improvements on highly heterogeneous data. Finally, privacy analysis suggests that SFL-PDA entails a reduced risk of privacy leakage.

## Some Sample Results
<p align="center">
<img width="85%" alt="results1" src="https://github.com/user-attachments/assets/8b616285-6ffe-46ae-b2a4-ef6f3c05c311" />
</p>  
<p align="center">
  <img alt="convergence_curve_0 01" src="https://github.com/user-attachments/assets/ec4793a7-32b3-42c7-975a-8c0a473ec7db" width="32%">
  <img alt="convergence_curve_0 05" src="https://github.com/user-attachments/assets/a98b3f8e-d15e-4d62-850d-211a2a1cfa1b" width="32%">
  <img alt="convergence_curve_0 1" src="https://github.com/user-attachments/assets/18d057f6-9dac-4a94-a144-5f976f395522" width="32%">
</p>

We will release our code after the paper is published.
