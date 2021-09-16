# ChIP_seq_test
ChIP-seq test assignment code,results and supplementary 

Greetings!
Here you can find test assignent for ChIP-Seq data analysis and obtained results.

# 1. Test assigment
  1. Download the chip-seq for the YY1 transcription factor as a bed file in broad or narrow peaks format from the ENCODE database.
  2. Select Top1000 best peaks based on -log pvalue.
  3. For selected top1000 peaks perform de novo motif discovery using Homer.
  4. Visually present the results obtained for the found motives based on Homer (you can use graphic materials obtained as a result of the Homer software). Write an   analytical commentary with biological interpretation  based on data from the literature and the Factorbook website.
  5. Perform GO enrichment for genes obtained by allocating a peak-gene using the GREAT tool and by assigning a peak to the nearest gene with a + - chain (for example, using bedtools)

# 2. Repo structure
  - GREAT_res : GO enrichment results made with GREAT tool;
  - HOMER_motif_search_res: results for GO analysis made with file after annotatePeaks.pl, along with .html results for de novo motif discovery/ known motifs;
      + homer_de_novo_Results: results for de novo motif discovery. Contains .svg files with motifs logo, along with .html motif info and motif sequence;
      + knownResults:  results for known motifs found by HOMER. Contains .svg files with motifs logo, along with motif sequence;
      + 8_10_12_motifs: all 8bp/10bp/12bp-long motifs in a single file; 
      + all found motifs in 1 file 
      + all known motifs in 1 file;
      + HOMER findmotifs.pl log file.
  - bedtools_results. Contains results of GO analysis made with *bedtools closest* output, along with some intermediate files(exons extracted from total output, and file containing gene names only);
  - HOMER_annotation_results. Contains results of GO analysis made with *annotatePeaks.pl* output, along with some intermediate files(logs of *annotatePeaks.pl*, and file containing gene names only);
  - src_data: simple Jupyter notebook to extract top 1000 peaks based on qValue, along with data from ENCODE (GM12892 original file, extracted top 1000 peaks file, bed6 file for GREAT GO enrichment with removed header);
  
 # 3. Software and used data:
 - https://www.encodeproject.org/genes/7528/ All YY1 experiments for *Homo sapiens*;
 - https://www.encodeproject.org/experiments/ENCSR000BLT/ GM12892 experiment;
 - http://homer.ucsd.edu/homer/index.html HOMER tool;
 - great.stanford.edu/public/html/index.php GREAT tool;
 - http://geneontology.org/ Gene Onthology main site;
 - https://factorbook.org/ Factorbook;
 - https://bedtools.readthedocs.io/en/latest/ bedtools.
 
 Hope you find this correct and somewhat useful.  
 Looking forward for your replies!
 
