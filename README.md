# SoundStream++ Audio Demo


## Abstract
In this paper, we propose SoundStream++, a high-rate extension of the SoundStream codec, which is able to generate almost transparent quality audio at 16 kbps for wideband speech signals. SoundStream shows reasonably good performance at low bit-rates (e.g. around 9 kbps), but its performance does not improve much when using more bits for encoding the latent embeddings. Motivated by experimental results showing that neural audio codec performance is highly related to the characteristics of latent embeddings such as dimensionality, dependency, and probability density function shape, we propose a convolutional transformer architecture and an attention-based multi-scale latent decomposition method that significantly enhances codec performance when quantizing high-dimensional embeddings. 
Experimental results show the superiority of our proposed model over conventional approaches.
