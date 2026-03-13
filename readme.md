# Isochronous Sampling
This repository contains the code for the paper [Isochronous Fixed-Weight Sampling in Hardware](https://eprint.iacr.org/2026/218.pdf).

The files IsochronousSampling_X_Y are the top level entites, for cryptoscheme X and variant Y.
The supported cryptoschemes are NTRU-HPS, Streamlined NTRU Prime and Classic Mceliece.
All three come in a low-area and high-speed variant.

The folder masked/ contains the files for the masked implementations, also for the cryptoschemes NTRU-HPS, Streamlined NTRU Prime and Classic Mceliece.
The folder masked/adder/ contains the Sklansky adder, and masked/lib_v/ contain the HPC2 gadgets.

Testbenches are in the folder tb/.

# License

This project is licensed under the MIT License. An SBOM file is also provided with license and dependency information.

### Third-Party Dependencies

This repository makes use of third-party code:
* The HPC2 gadgets are from https://github.com/cassiersg/fullverif/
* The masked Sklansky adder and multiplexer are from https://github.com/AdrianMarotzke/Masked-SNTRUP
* The FIFO buffer is from https://vhdlwhiz.com/ring-buffer-fifo/ 

# Acknowledgments
This work was supported by the Federal Ministry of Research, Technology and Space (BMFTR) of the Federal Republic of Germany (grant 16KIS1572K, SASVI), as well as the  European Commission under the grant agreement number 101070374 (CONVOLVE).
This work was supported by the European Cybersecurity Competence Centre under the European Union’s Horizon Europe research and innovation program under  grant agreement number 101225859 (FOCAL).

# Citation
If you want to cite this work, please use the following bibtex:

```
@Misc{marotzke2026isochronous,
  title="{Isochronous Fixed-Weight Sampling in Hardware}",
  author={Marotzke, Adrian},
  year={2026},
  howpublished = "{Cryptology ePrint Archive, Report 2026/218}",
  url = {https://eprint.iacr.org/2026/218},
}
```