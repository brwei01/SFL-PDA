## About SFL-PDA (abstract of our work)
Self-supervised federated learning can leverage unlabeled data to alleviate representation-level data heterogeneity but remains limited in addressing label-level imbalance. While pre-trained generative models show promise for augmenting minority-labelled data, their effectiveness diminishes in real-world FL scenarios, where client data is private and must not be exposed to the public. To fill this gap, we propose SFL-PDA (*Self-supervised Federated Learning with Personalized Diffusion Adapter*) to address data heterogeneity at both representation- and label-levels. SFL-PDA designs a lightweight class-conditioned LoRA adapter to finetune a personalized diffusion model as per client requests. In this way, the client’s diffusion model can effectively capture private, domain-specific characteristics for personalized minority-class data generation, ensuring SFL is collaboratively trained with balanced labeled data and achieves consistent performance.  We evaluate SFL-PDA on two standard benchmarks and one private domain-specific dataset against various state-of-the-art baselines under varying heterogeneity levels. The results demonstrate that SFL-PDA can effectively address data heterogeneity, especially at severe levels. Furthermore, ablation studies confirm that our proposed class-conditioned LoRA adapter can yield up to 28.5% improvements on highly heterogeneous data. Finally, privacy analysis suggests that SFL-PDA entails a reduced risk of privacy leakage.

## Some Sample Results
<img width="1057" height="719" alt="results1" src="https://github.com/user-attachments/assets/6d56a2d6-ea7d-4c9b-8c70-547ae5d539f2" />
![convergence_curve_0 01](https://github.com/user-attachments/assets/bc04e670-4bd7-4630-845f-7be48a546efb)
![convergence_curve_0 05](https://github.com/user-attachments/assets/8e5e095d-5bd1-4962-abae-ec5210128975)
![convergence_curve_0 1](https://github.com/user-attachments/assets/69579f5f-883d-453c-ad1f-0763b853040c)


We will release our code after the paper is published.
