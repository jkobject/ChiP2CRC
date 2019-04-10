# Chip to CRC

Here I try to reimplement some of the code leading to the identification of enhancers, super enhancers, and the core regulatory circuitry of the cell according to H3K7me3 marks from CHip-seq datasets of human cell lines.


## How to run the code

Just have python installed together with jupyter, and run the jupyter [.ipynb file](https://github.com/jkobject/ChiP2CRC/blob/master/from%20ChiP%20to%20Core%20Regulatory%20Circuitry.ipynb).


## The output

Amongst all, this code extracts informations such as:
- the name of the [enhancers](https://github.com/jkobject/ChiP2CRC/tree/master/peak_called/peak_called/NA_summits_AllEnhancers.table.txt), [super enhancers](https://github.com/jkobject/ChiP2CRC/tree/master/peak_called/peak_called/NA_summits_SuperEnhancers.table.txt) of the cell, as well as their binding profile [1](https://github.com/jkobject/ChiP2CRC/tree/master/coverage.bw) and [2](https://github.com/jkobject/ChiP2CRC/tree/master/peak_called/peak_called/NA_summits_Gateway_SuperEnhancers.bed) . 
- A Model of the CRC containing the [Core genes](https://github.com/jkobject/ChiP2CRC/tree/master/crcmapper/crcmapperCRC_AUTOREG.txt) involved in the regulatory circuitry as well as their related [secondary genes](https://github.com/jkobject/ChiP2CRC/tree/master/crcmapper/crcmapperCRC_SE_ASSIGNMENT_GENE.txt) and overall [expressed genes](https://github.com/jkobject/ChiP2CRC/tree/master/crcmapper/crcmapperCRC_EXPRESSED_GENES.txt).
- A binding pattern (_CRC_motifs.bed files_) for these core genes. 
- An average [binding profile](https://github.com/jkobject/ChiP2CRC/tree/master/peak_called/NA_model.pdf) of the peak model over the sequences.
- A [plot](https://github.com/jkobject/ChiP2CRC/tree/master/superenhancers/NA_summits_Plot_points.png) of the enhancers [sorted](Nhttps://github.com/jkobject/ChiP2CRC/tree/master/superenhancers/A_summits_AllEnhancers.table.txt) by the average strength of their signal (confirming the X firsts as being super enhancers).



*This code follows on works from the Young Lab, MACS2 community and uses Bowtie, samtools and Meme. 




under MIT licence
@jkobject
Jérémie Kalfon
www.jkobject.com