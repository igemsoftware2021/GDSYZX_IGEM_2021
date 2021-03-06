# GDSYZX
<h1>qtWGCNA: A <strong>Qt</strong> compiled interface for </strong>WGCNA</strong> analyses</h1>

Currently, qtWGCNA (v 1.0) is under its first version development. As showed in the below figure, the framework of qtWGCNA relies on a Qt-based fore-end and the back-end python script of iterativeWGCNA [1].
<p style="text-align: center">
  <img src="https://2021.igem.org/wiki/images/5/58/T--GDSYZX--qtWGCNA.png" width="900px"  alt="" />
  </p>

<h2>1. Quick Start</h2>
  qtWGCNA is developed as an interface of iterativeWGCNA python script, to run qtWGCNA, we can use WSL of Windows 10 (can be downloaded and installed from Microsoft store) or run command './qtWGCNA' (in <strong>build-qtWGCNA-Desktop-Release/</strong>) on a linux server terminal. We recommend downloading WSL from Microsoft store in Win 10 system because it is more light weight and no requirement for complicated coding skills.

  <p style="text-align: center">
  <img src="https://2021.igem.org/wiki/images/4/45/T--GDSYZX--WSL.png" width="900px"  alt="" />
  </p>

  After WSL or server deployment, qtWGCNA required miniconda environment to install iterativeWGCNA by running commandline 'conda install -c conda-forge iterativewgcna' (https://anaconda.org/conda-forge/iterativewgcna). More information about how to install Miniconda, <a href="https://docs.conda.io/en/latest/miniconda.html" target="_blank"><u>please click me.</u></a>
  Finally, by uoload the gene expression file (<a href="https://github.com/cstoeckert/iterativeWGCNA/blob/master/README.md#input-file-format" target="_blank"><u>file format info</u></a>) with 'browse' button and set required parameters, we are able to run iterativeWGCNA at the back-end and wait for the processing to be done!
  
<h2>2. Interface Options</h2>
  Currently, qtWGCNA is now allowed to accept all arguments of valid for the WGCNA blockwiseModules R function (<a href="https://www.rdocumentation.org/packages/WGCNA/versions/1.70-3/topics/blockwiseModules" target="_blank"><u>blockwiseModules help document</u></a>). More information about the customized parameters, e.g. soft power or network type, please refer to WGCNA parameters.

<h2>3. Results and logs</h2>
A main text and log result of qtWGCNA was showed as below, which indicates how much connected of all the co-expressed genes in well-divided WGCNA modules.
  <p style="text-align: center">
  <img src="https://2021.igem.org/wiki/images/4/40/T--GDSYZX--software-fig3.png" width="900px"  alt="" />
  </p>
   <p style="text-align: center">
  <img src="https://2021.igem.org/wiki/images/5/54/T--GDSYZX--software-fig4.png" width="900px"  alt="" />
  </p>
  
A main figure result of qtWGCNA was showed as below, which indicates how many genes are jointly co-expressed.
  ![alt text](https://2021.igem.org/wiki/images/0/0f/T--GDSYZX--software-video-fig2.png)
  <p>More information about the output files, please refer to <a href="https://github.com/cstoeckert/iterativeWGCNA/blob/master/README.md#output-files" target="_blank"><u>iterativeWGCNA output files</u></a></p>
  
 <h2>4. Source Code</h2>
  The source code of qtWGCNA can be compiled by Qt creator. It is also available in our wiki page: https://2021.igem.org/Team:GDSYZX/Software#section4
  <p style="text-align: center">
  <img src="https://2021.igem.org/wiki/images/e/e2/T--GDSYZX--qtcreator.png" width="900px"  alt="" />
  </p>
  

[1] iterativeWGCNA: iterative refinement to improve module detection from WGCNA co-expression networks Emily Greenfest-Allen, Jean-Philippe Cartailler, Mark A. Magnuson, Christian J. Stoeckert Jr. bioRxiv 234062; doi: https://doi.org/10.1101/234062.
