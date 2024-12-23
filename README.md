This repo hosts the practical implementation of the journal paper [“Cross-Correlated Scenario Generation for Renewable-Rich Power Systems Using Implicit Generative Models”, Energies, 16(4), 2023](https://www.mdpi.com/1996-1073/16/4/1636), specifically the C<sup>2</sup>RGAN model, trained using a publicly available dataset from Huggingface (a different, propietary dataset was used in the original paper)

### Paper Abstract

> Generation of realistic scenarios is an important prerequisite for analyzing the reliability of renewable-rich power systems. This paper satisfies this need by presenting an end-to-end model-free approach for creating representative power system scenarios on a seasonal basis. A conditional recurrent generative adversarial network serves as the main engine for scenario generation. Compared to prior scenario generation models that treated the variables independently or focused on short-term forecasting, the proposed implicit generative model effectively captures the cross-correlations that exist between the variables considering long-term planning. The validity of the scenarios generated using the proposed approach is demonstrated through extensive statistical evaluation and investigation of end-application results. It is shown that analysis of abnormal scenarios, which is more critical for power system resource planning, benefits the most from cross-correlated scenario generation.

This repo contains the code to train the C<sup>2</sup>RGAN model, althout it doesn't explore the conditional training of the model nor the separation of dataset on the basis of Dynamic Time Warping.

Dataset: https://huggingface.co/datasets/vitaliy-sharandin/energy-consumption-hourly-spain