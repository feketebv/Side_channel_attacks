# Side_channel_attacks
* Hweight_dpa_sca_aes_sbox.py : A schoolbook example of differential power analysis side channel analysis of Advanced Encryption Standard's S-box based hacking.
* Hdist_dpa_sca_aes_sbox.py : Roughly the same, but with Hamming distances being considered as the primary leakage source.
* Hweight_dpa_sca_16x_aes_sbox.py : A more near life solution where multiple S-box computations comprise the leakage. As such, the example also shows, that this attack works in the presence of noise, because when the input of a particular S-box is being guessed, all other S-box substitutions are meaningless (algorithmic) noise in the leakage data.
* Hweight_dpa_sca_16x_aes_sbox_PYCUDA.py : A GPU translatable version of the previous one, that works roughly 57x faster ie. performs the correlations in roughly 0.8sec instead of 47sec on Nvidia Geforce GTX 1050 vs. Intel Core i5-7300HQ respectively. The code is fairly simple but needs the proprietary Anaconda compiler for Nvidia GPUs (https://www.anaconda.com/products/individual).
